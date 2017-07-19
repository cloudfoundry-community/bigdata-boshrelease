# FIXES
- put the log data that kafka stream into a directory on a BOSH managed persistent disk. This is a backwards incompatible change but neccessary for a kafka broker to keep its data when a vm goes away.
