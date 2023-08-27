So, what is this you may be asking -- well, this is a modified open source audio hal that is designed to work for lg devices which feature an ess dac. This hal can theoretically work for other devices which feature a dac
on the msm8996/msm8998 platform. To trigger the ess dac, audio must be paused for 3-5 seconds, after which the dac routes will kick in.

Features:

-Automatic route/backend switching

-Dac status

-Native support for upto 3 dac routes

-Allows for both WCDxxxx and dac operation

-Doesn't rely on any stock relics or hacks to function.

Note:
Requires dac panel to interface with the hal. (i suppose you could create your own way to mess with the props, up to you)
https://github.com/LGE-G5-G6-V20/android_hardware_lge/tree/lineage-20/dac_panel


Tested on:
V20 - es9218
