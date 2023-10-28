# mkosi-koji

A set of [mkosi](https://github.com/systemd/mkosi/) configuration files to build
an image with koji installed and configured for local testing. By default, koji
will be installed from the official fedora repositories. To build the koji rpm
from source, add a file `mkosi.local.conf` with the following contents:

```conf
[Content]
BuildSources=<path-to-koji-sources>:koji
```
