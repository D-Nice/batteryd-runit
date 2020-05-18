# batteryd

Runit service for monitoring your battery levels if discharging,
sending notifications and suspending when below configured thresholds.

## Requirements

- X Session
- libnotify
- A battery ;P

## Install

```sh
mkdir -p /etc/sv/batteryd
cp -r ./* /etc/sv/batteryd
```

ensure root is owner and group...

## Configuration

Check conf file for available and settable configurables.

## Notes

Should be reusable even if you don't have a runit specific system

If you're missing the notifications lib, you can disable the strict exit
code checking by commenting out `set -e`.

May also contain useful parts, such as a
portable way for notifying all users with active DISPLAY.
