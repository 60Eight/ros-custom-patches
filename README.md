Custom patches for use with [rattlesnakeos-stack](https://github.com/dan-v/rattlesnakeos-stack) to build [RattleSnakeOS](https://github.com/RattlesnakeOS).  

## How to
Add the following to end of your `rattlesnakeos-stack` config file.
```
...

[[custom-patches]]
  repo = "https://github.com/60Eight/ros-custom-patches"
  patches = [
      "00001-global-internet-permission-toggle.patch",
      "00002-global-sensors-permission-toggle.patch",
      "00003-disable-menu-entries-in-recovery.patch",
      "00004-increase-default-maximum-password-length.patch",
      "00006-enable-powersaving-features.patch",
      "00008-disable-supl-agps.patch",
      "99999-microg-sigspoof.patch"
  ]

...
  
```

## References:
- https://github.com/dan-v/rattlesnakeos-stack#patches-and-scripts
