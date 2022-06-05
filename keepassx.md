KEEPASS
=======

Much to the bane of any security department, Keypass is used everywhere.. serioiusly.  There are of course a few issues.

Due to the  design of the the database format,  it contains unique and unecrypted fields.  One of which is bytes[0-12] in the heaader.

|bytse|what|
|----- | --------------------------|
|4 |   magic - [0x03,0xD9,0xA2,0x9A]|
|4 |   version. (LE uint32)|
|2 |   major_version. (LE uint16)|
|2   | minor_version. (LE uint16) |
------------------------------------


As a result idenifying what should be a secret becomes trivial.  There is a sha256 checksum and hmac however they are blindlly trusted before reading nor validating any key.


KeepassX supports an online version check .. which is hosted on Github, every 7 days by default.
https://github.com/keepassxreboot/keepassxc/blob/b5e0572155594cfa08bbfc8dd9b4447085c21e97/src/updatecheck/UpdateChecker.cpp#L58

There is no verification on the data received rather it's existance in the repo.  Thus anyone with comit permissions can compromise everyone.

That is not something you want in your password vault.

