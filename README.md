# Kotori PHP CLI
Just a simple CLI scffold tool for the PHP framework Kotori.php, you can use it for scaffolding Kotori.php projects.

## Installation
Kotori.php CLI requires PHP(>=5.5) and composer installed on your environment.

```shell
$ composer global require kasumi/kotori-php-cli:dev-master
```

Make sure that you have added composer global vendor bin directory to your **PATH**.

Let's take Linux for example:
```shell
$ export PATH="$HOME/.composer/vendor/bin:$PATH"
```

## Usage
```shell
$ kotori <command> [arg1] [arg2]...
```

Here are some examples:

```shell
# initialize a pure Kotori.php project
$ kotori init
$ kotori i vendor/name

# modify config
$ kotori config <set|set-array|remove|list|reset>

# generate a pure controller/model named Hello
$ kotori generate controller Hello
$ kotori g model Hello

# start a dev server on localhost:8000
$ kotori serve --port 8000

# import or export database
$ kotori db export db_instance_name ./db.sql
$ kotori db import db_instance_name ./db.sql
```
Other commands and detailed usage can be found by executing ```kotori help``` command.

## License
Apache v2
