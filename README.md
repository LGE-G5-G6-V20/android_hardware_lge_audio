So, what is this you may be asking -- well, this is a modified open source audio hal that is designed to work for lg devices which feature an ess dac. This takes a different approach from stock, which contained all of the additional dac control functions within the hal. My approach is different from theirs. The goal of my approach is to let the hal just handle the audio routing and modify the ess driver to expose sysfs nodes, of which will be manipulated and controlled through scripts, controlled by my added properties. This could also theoretically be used for other devices which use a dac, however I do not care about porting it to said devices.

Working features:
-Audio routing

WIP features: 
-AVC volume
-High impedence
-Adjustable bitrate
-Adjustable filters
-Adjustable presets

Tested on:
V20 - es9218P

Needed commits:(Bound to change over time)

https://github.com/LGE-G5-G6-V20/android_device_lge_v20-common/commit/148fc99ae3a8e7012546403f846ff5fe2ab523e9

https://github.com/LGE-G5-G6-V20/android_device_lge_v20-common/commit/df42f3e6f435ba92e6d350ecadda548204eede89

https://github.com/LGE-G5-G6-V20/android_device_lge_msm8996-common/commit/9c0ddca14afa6264cd244c201366b88fdb8aa4e1
