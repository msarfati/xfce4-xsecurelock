# xfce4-xsecurelock
Michael Sarfati (michael.sarfati@utoronto.ca)
Thu Apr 14 00:39:04 EDT 2016

## What it does
Eases the integration of [XSecurelock](https://github.com/google/xsecurelock) with the [XFCE4 desktop environment](www.xfce.org). This is merely a script invoked by `xflock4`

## Installation

1. `make install` -- this copies `xfce4-xsecurelock-script.bash` to `/usr/local/bin/xflock4`

2. Invoke ctrl-alt-delete or suspend to test xsecurelock.

## Caveats

This installation is *very* basic. You can customize `xsecurelock` for different parameters. See [XSecureLock Setup](https://github.com/google/xsecurelock#setup).

## Troubleshooting

### Locking / Suspending isn't calling XSecureLock

1. Make sure you've installed `xsecurelock`

2. Make sure you don't have any other locking/screensaver applications installed.

3. Inspect your `$PATH` -- make sure that `/usr/local/bin` is before `/usr/bin`
You can do this by typing the following into the terminal:
```
echo $PATH
```
and make sure that `/usr/local/bin`

## Links
* [How to change lock screen for xfce?](https://www.reddit.com/r/xfce/comments/1lit6s/how_to_change_lock_screen_for_xfce/)

