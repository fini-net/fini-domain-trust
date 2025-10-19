# FINI Domain Trust

[![Open Source Love png2](https://badges.frapsoft.com/os/v2/open-source.png?v=103)](https://github.com/ellerbrock/open-source-badges/)
[![GPLv2 license](https://img.shields.io/badge/License-GPLv2-blue.svg)](https://github.com/fini-net/fini-domain-trust/blob/master/LICENSE)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/fini-net/fini-domain-trust/graphs/commit-activity)

The FINI Domain Trust is here to keep good domains from bad hands.

## Preview

You can preview it at https://fini-net.github.io/fini-domain-trust/ but currently it looks terrible.

## Hugo/Theme updates

Hugo probably got upgraded with `brew upgrade` at some point so you will
want to run:

```ShellCommand
git submodule update --remote themes/ananke
```

to get the submodule current so that `hugo` runs cleanly.
