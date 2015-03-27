# cliPublish

## Introduction

cliPublish allows easily uploading a file to a fixed directory of your
webserver using rsync. On success it prints the URL the file will be available
at.

## Usage
You need to create a small config file in `~/.config/cliPublish/remotes.conf`.
There is an example file in [doc/remotes.conf](doc/remotes.conf).

## Example

```
$ cliPublish.py 20140903_0399.JPG
20140903_0399.JPG
        310,428 100%  264.80MB/s    0:00:00 (xfr#1, to-chk=0/1)
http://tmp.mheistermann.de/20140903_0399.JPG
```

Optionally you can also specify a filename for the remote side:

```
$ cliPublish.py 20140903_0399.JPG ijen_crater.jpg
20140903_0399.JPG
        310,428 100%  264.80MB/s    0:00:00 (xfr#1, to-chk=0/1)
http://tmp.mheistermann.de/ijen_crater.jpg
```

## License

cliPublish was written by Martin Heistermann <github()mheistermann.de>
and is available under the terms of the GPL v3.



## Ideas

* Support multiple servers in config, select using optional argument
* Warn/Stop/Backup if remote filename already exists
* Upload multiple files at once, creating a directory with an index.html

## Contributing

Send me a pull request on github or [email me a patch](mailto:github[]mheistermann.de).
