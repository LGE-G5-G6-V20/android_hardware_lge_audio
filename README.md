This is a modified open source audio hal that is designed to work for lg devices which feature an ess dac. 
This hal can theoretically work for other devices which feature a dac

on the msm8996/msm8998 platform. To trigger the ess dac, audio must be paused for 3-5 seconds, after which the dac routes will kick in.

Features:

-Automatic route/backend switching

-Dac status

-Native support for upto 5 dac "modes" (really just routes in the eyes of the hal)

    -NORMAL
  
    -HIGH IMPEDANCE
  
    -AUX HIGH IMPEDANCE (refer to ess datasheet for difference about H.Imp & aux H.Imp)
  
    -24 BIT HIGH IMPEDANCE
  
    -24 BIT AUX HIGH IMPEDANCE
  

-Allows for both WCDxxxx and dac operation

-Doesn't rely on any stock relics or hacks to function.

Note:
Requires dac panel to interface with the hal. (i suppose you could create your own way to mess with the props, up to you)
https://github.com/LGE-G5-G6-V20/android_hardware_lge/tree/lineage-20/dac_panel


Tested on:
V20 - es9218