Yes, you can protect Shadow Daemon with itself. I would love to say that I am sure that the web interface has no bugs, but the truth is that I rely on a lot of third party libs and I can not guarantee that all of them are secure as well. So always be prepared!

shadowd_ui uses a front controller, so every request is routed through one file (the default caller). To use this rules you have to change *caller* to *PHP_SELF* in your connector configuration file.

The rules are very tight and a good example for how rules should look like. There is really no room for vulnerabilities.
