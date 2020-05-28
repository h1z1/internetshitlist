GITHUB uBlock Rules
--------------------

Github is not surprisingly annoying by default

```
!!! Github
||api.github.com^$ping
||github.com/users/*/hovercard$xhr,1p
||collector.githubapp.com^

! I am not a test subject..
!!! ||github.com/users/h1z1/feature_preview/indicator_check.json$xhr,1p,important
||github.com/users/*/feature_preview/indicator_check.json$xhr,1p,important

! Really Github?
github.com##.js-notice.mb-3.mt-0.mt-md-3
github.com##.js-notice.mb-4.flash-warn.flash

github.com##.box-shadow-large.Box.mt-6.p-3.text-left.Popover-message--large.Popover-message--top-left.Popover-message
github.com##div.js-notice:nth-of-type(1)
github.com##.bg-white.js-notice

github.com###issuecomment-560020167 > .reorderable-task-lists.timeline-comment--caret.js-comment.js-task-list-container.previewable-edit.comment.unminimized-comment.timeline-comment.ml-n3 > .js-edit-comment-hide.edit-comment-hide > .js-updatable-content.js-socket-channel.js-reactions-container.has-reactions.border-top.comment-reactions

github.com##.mt-3.mb-3
github.com##.position-relative.Popover
github.com##.d-flex.mb-4.p-3.Box
github.com##.js-issue-xrefs-new-feature-notice.mb-5.position-absolute.Popover
github.com##.p-2.border-bottom.js-notice
github.com##.text-md-left.text-center.flex-md-justify-start.flex-justify-center.flex-items-center.flex-wrap.d-flex

!!! - Github
```
