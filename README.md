# sowm-flexipatch

A build of sowm that makes it easier to apply patches.

## About

Similar to the flexipatch builds made by [bakkeby](https://github.com/bakkeby), sowm-flexipatch aims to make the patching process
of [sowm](https://github.com/dylanaraps/sowm) easier by using preprocessor directives to decide which patches get included during build time. Some patches have been modified to avoid malfunctions or conflicts with other patches, these will have `_mod`
appended to their names inside the `patches/` directory.

## Usage

To decide which patches get included, the `patches.h` file needs to be modified.
```c
#define PATCH_NAME 0
```

> Changing the value next to the patch name to `1` will include it during build time.
