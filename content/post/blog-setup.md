---
title: "Blog Setup"
date: 2021-08-15T07:30:45-07:00
tag: [notes]
---

1. make bucket, enable public, static sharing, add bucket policy to arn of bucket self
1. index.html text/html; charset=utf-8
1. terraform delegation zone id
1. export AWS_PROFILE=drake1
1. dns alias=true
1. hugo server
1. hugo
1. hugo deploy
1. hugo new site drakeblog
1. git submodule add https://github.com/zwbetz-gh/cupper-hugo-theme.git themes/cupper-hugo-theme
1. echo theme = \"cupper-hugo-theme\" >> config.toml 
1. `hugo new post/markdown-lesson/index.md` and don't forget replace draft = tags: [something]
1. 
```
[deployment]
# By default, files are uploaded in an arbitrary order.
# Files that match the regular expressions in the "Order" list
# will be uploaded first, in the listed order.
order = [".jpg$", ".gif$"]


[[deployment.targets]]
# An arbitrary name for this target.
name = "drakeCv"

# S3; see https://gocloud.dev/howto/blob/#s3
# For S3-compatible endpoints, see https://gocloud.dev/howto/blob/#s3-compatible
URL = "s3://cv.drakenor.com?region=us-west-1"
```