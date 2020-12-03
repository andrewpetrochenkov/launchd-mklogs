<!--
https://readme42.com
-->



[![](https://img.shields.io/badge/OS-Unix-blue.svg?longCache=True)]()
[![](https://img.shields.io/pypi/v/launchd-mklogs.svg?maxAge=3600)](https://pypi.org/project/launchd-mklogs/)
[![](https://img.shields.io/npm/v/launchd-mklogs.svg?maxAge=3600)](https://www.npmjs.com/package/launchd-mklogs)[![](https://img.shields.io/badge/License-Unlicense-blue.svg?longCache=True)](https://unlicense.org/)
[![](https://github.com/andrewp-as-is/launchd-mklogs/workflows/tests42/badge.svg)](https://github.com/andrewp-as-is/launchd-mklogs/actions)

### Installation
```bash
$ [sudo] pip install launchd-mklogs
```

```bash
$ [sudo] npm i -g launchd-mklogs
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

#### Examples
```bash
$ find ~/Library/LaunchAgents -name "*.plist" -print0 | xargs -0 launchd-mklogs
```

<p align="center">
    <a href="https://readme42.com/">readme42.com</a>
</p>
