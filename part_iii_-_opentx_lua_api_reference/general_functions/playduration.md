# playDuration\(duration \[, hourFormat\]\)

Play a time value \(text to speech\)

@status current Introduced in 2.1.0

### Parameters

* `duration` \(number\) number of seconds to play. Only integral part is used.
* `hourFormat` \(number\):
  * `0 or not present` play format: minutes and seconds.
  * `!= 0` play format: hours, minutes and seconds.

### Return value

none

## Examples

The one time script below will announce "zero hours 1 minute and 1 second"

```lua
local function run()
  playDuration(61, 1) -- announce "zero hours 1 minute and 1 second
  return 1
end

return { run=run }
```
