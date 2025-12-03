# FINI Domain Trust

[![Open Source Love png2](https://badges.frapsoft.com/os/v2/open-source.png?v=103)](https://github.com/ellerbrock/open-source-badges/)
[![GPLv2 license](https://img.shields.io/badge/License-GPLv2-blue.svg)](https://github.com/fini-net/fini-domain-trust/blob/master/LICENSE)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/fini-net/fini-domain-trust/graphs/commit-activity)

The FINI Domain Trust is here to keep good domains from bad hands.

## Sites

These sites are part of the FINI Domain Trust in December 2025:

- <https://www.almanacvapolitics.org>
- <https://www.bettywalls.com>
- <https://www.gasp.org>
- <https://www.hangmansdaughter.org>
- <https://www.hrlug.org>
- <https://www.partnersforjustice.com>
- <https://www.perlclass.org>
- <https://www.perlclasses.org>
- <https://www.politicsvirginia.org>
- <https://www.seaprojects.org>
- <https://www.vccinc.net>

## Hugo/Theme updates

Hugo probably got upgraded with `brew upgrade` at some point so you will
want to run:

```ShellCommand
git submodule update --remote themes/ananke
```

to get the submodule current so that `hugo` runs cleanly.

- TODO: modernize to get rid of the submodule

## Service via Digital Ocean App Platform

You can see the [terraform we used](https://github.com/fini-net/fini-infra/tree/main/l6_ingress/app-fini-domain-trust)
to serve these sites using the Digital Ocean App Platform.
