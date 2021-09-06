# sowm-flexipatch

A build of sowm that makes it easier to apply patches.

## About

Similar to the flexipatch builds made by [bakkeby](https://github.com/bakkeby),
sowm-flexipatch aims to make the process of patching
[sowm](https://github.com/dylanaraps/sowm) easier by using preprocessor
directives to decide which patches get included during build time. Some patches
have been modified to avoid malfunctions or conflicts with other patches, these
will have `_mod` appended to their names inside the `patches/` directory.

## Usage

To decide which patches get included, the `patches.h` file needs to be modified.
```c
#define PATCH_NAME 0
```

> Changing the value next to the patch name to `1` will include it during build time.

## Patches

The patches listed below are the ones that are currently included.

<details>
    <summary>From the (archived) <a href="https://github.com/dylanaraps/sowm-patches">patches repository</a>:</summary>
    <br>
    <ul>
        <a href="https://github.com/dylanaraps/sowm-patches/blob/master/patches/sowm-normal-kill.patch"><li>Normal Kill</li></a>
    </ul>
</details>

<details>
    <summary>From the <a href="https://github.com/dylanaraps/sowm/pulls">pull requests</a>:</summary>
    <br>
    <ul>
        <a href="https://github.com/dylanaraps/sowm/pull/57"><li>Titlebars</li></a>
    </ul>
</details>

## Learn More

* [sowm](https://github.com/dylanaraps/sowm)
* [Original Flexipatch Idea](https://github.com/bakkeby)
* [What is an X window manager?](https://en.wikipedia.org/wiki/X_window_manager)
* [What even is patching?](https://www.youtube.com/watch?v=-CiLU9-RAGk)
