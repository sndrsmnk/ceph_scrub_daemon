# ceph_scrub_daemon
Ceph (deep) scrub daemon

This **far from done** "Ceph Scrub Daemon" fires off scrubs on PGs and prioritizes PGs by `last(_deep)_scrub` timestamp.

It tries to limit the number of simultaneous scrubs, but this logic may well be flawed.

Runs shallow scrubs by default. Use the `-D` or `--deep-scrub` argument to make it run deep scrubs.
