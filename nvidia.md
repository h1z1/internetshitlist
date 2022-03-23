NVIDIA
------

Not really worth documenting them all but there are many reasons to distrust NVIDIA directly.

Documenting some very recent events however have underlined the need for caution.

1) There are exploits STILL in the wild against their drivers, specifically h264/265 encoders.  They have been used during "conflicts" for reasons I can only imagine.  Two sites where this happens is Twitch, and Google.  The gist of it is the attack(s) can crash / compromise the host, through the bitstream directly.

NVIDIA rather quietly released an update post "J6", but did not address them all.


2) NVIDIA's driver and/or entire code base was "leaked".  The intent of this is unclear but there have already been more attacks against NVIDIA drivers since including the certificates used to sign them.

A rather ironic twist to this is their response including hacking the group who did the initial breach - by using their drivers.  Not cool.

3) NVIDIA STILL refuses to address IOMMU isolation.  P2P Mem (aka RDMA), will not work without disabling IOMMU. This has been reported to NVIDIA through the years including by myself.
Some examples (links scrubed to not tag them ) 

- https://github.com[space]/NVIDIA/nccl-tests/issues/18
- https://github.com[space]/NVIDIA/cuda-samples/issues/48

etc.


NVIDA overall takes - or at least did - an extreme hate based response to Virtualization leading to ugly hacks with QEMU spoofing (See the _many_ threads regarding "error 43")  Rather ironic. 

From a security standpoint (and corporate), GeForce "experience" is a whole other can of worms to avoid, as is Shadow Play.

More to come.

---
* Breach details regarding the group and links deliberately left out.  Google it.
