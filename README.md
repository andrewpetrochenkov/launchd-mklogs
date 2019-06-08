<!--
https://pypi.org/project/readme-generator/
https://pypi.org/project/python-readme-generator/
-->

[![](https://img.shields.io/badge/OS-Unix-blue.svg?longCache=True)]()
[![](https://img.shields.io/pypi/v/launchd-mklogs.svg?maxAge=3600)](https://pypi.org/project/launchd-mklogs/)
[![](https://img.shields.io/npm/v/launchd-mklogs.svg?maxAge=3600)](https://www.npmjs.com/package/launchd-mklogs)
[![Travis](https://api.travis-ci.org/looking-for-a-job/launchd-mklogs.svg?branch=master)](https://travis-ci.org/looking-for-a-job/launchd-mklogs/)

#### Installation
```bash
$ [sudo] npm i -g launchd-mklogs
```
```bash
$ [sudo] pip install launchd-mklogs
```

#### How it works
`launchd.plist`
```xml
<key>StandardErrorPath</key>
<string>path/to/err.log</string>
<key>StandardOutPath</key>
<string>path/to/out.log</string>
```

`launchd-mklogs` will create `StandardErrorPath`, `StandardOutPath` directories and files with current user permissions

#### Scripts usage
command|`usage`
-|-
`launchd-mklogs` |`usage: launchd-mklogs path ...`

#### Examples
```bash
$ find ~/Library/LaunchAgents -name "*.plist" -print0 | xargs -0 launchd-mklogs
```

<p align="center">
    <a href="https://pypi.org/project/python-readme-generator/">python-readme-generator</a>
</p>