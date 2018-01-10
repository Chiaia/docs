---
permalink: /commands/general/
title: General Commands
---

### showfps
```
showfps [#]
```
Shows or hides the framerate display.

##### Accepted Values

| Value | Description |
|:---|:---|
| `0` | Framerate display hidden |
| `1` | Framerate display visible |

**Tip:** Using `showfps` without a parameter toggles visibility.
{: .notice--info}

### fps_position
```
fps_position <x> <y>
```
Repositions the framerate display.

### screenshot
```
screenshot <format> [hide]
```
Takes a screenshot in the specified format.

Supported formats: `bmp`, `jpg`, `png`

If specified, the optional `hide` parameter hides Windower objects from the screenshot.

### video start
```
video start <xres> <yres> <fps> <quality>
```
Starts recording a video with the specified parameters.

### video stop
```
video stop
```
Stops video recording.

### wait / pause
```
wait <#>
pause <#>
```
Pauses execution of a command, bind, alias, or script for the given number of seconds. Decimal values may be used.

## Alias Commands

### alias
```
alias <alias> <command>
```
Creates a pseudo console command that can be typed into the console or used in a script or key bind.

For example: `alias blah wait 5;echo hello` creates the `blah` pseudo-command.

### clearaliases
```
clearaliases
```
Clears all currently-defined aliases.

### listaliases
```
listaliases
```
Lists all currently-defined aliases.
The command may fail if you have more than 40 aliases.
