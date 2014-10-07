Public History
--------------

Makes it easy to publish your bash history line by line in real-time to a web server. Good for live tutorial sessions or other teaching. Note: works best if you have SSH key login to the server [like this](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys--2).

public-history is invoked with one command of this form
```bash
$ source enable_logging <file> <server> "<path_on_server>"
```

A complete demo looks like this
```bash
$ source enable_logging ~/index.html www.myserver.com "~/public_html/demo/index.html"
$ echo This will show up on the public page in real-time!
$ ls -d */ # lists all directories
$ echo That's all for now!
$ source disable_logging
```
