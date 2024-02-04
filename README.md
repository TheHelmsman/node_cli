# Configuration files creator.

Simple node.js application that shows how to work with `commander` and `inquirer` npm modules to build basic node CLI application

## Dependencies:

`node version:` ^16.0.0

## Setup

1. Get app code fro repository

```bash
git clone
```

2. Install node modules:

```bash
npm install
```

3. Check if application works - get app version:

```bash
npm run ver
```

Sample output:

```bash

> nodejs_cli@1.0.0 ver
> node app.cjs --version

1.0.0
```

4. Run app without params or with help parm to get information on usage:

```bash
npm run start
```

Sample output:

```bash

> nodejs_cli@1.0.0 start
> node app.cjs

Usage: app [options] [command]

Configuration files creator.

Options:
  -V, --version              output the version number
  -h, --help                 display help for command

Commands:
  create|c [options] <name>  Create new configuration file.
  all|a                      Show all configuration files.
  help [command]             display help for command
```

5. Run application with startup params to create configuration file:

```bash
npm run start c json test.json
```

Fill all prompt querries and check result in `files` folder:

Sample output:

```bash

> nodejs_cli@1.0.0 start
> node app.cjs

? Charset:  utf-8
? Max RAM usage, Mb:  1024
? Max CPU usage, %:  10
? Updates interval, ms:  1000
? Processes count:  5

File "json.cfg" created.
```
