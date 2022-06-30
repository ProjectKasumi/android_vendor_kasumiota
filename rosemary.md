This OTA is going to be an optimization update, in which I have added
2 props that will tell HWUI to focus more on GPU and less on CPU for
graphical processing.

Another change is rather interesting. I personally thought the content
on AOD shifts in a little radius and not too far away. It apparently
does, which has been sorted out now.

Thanks to @aScordino for his recommendations and reference commits on
these!

And also, you can consider this update as a last-day-of-pride-month
update, given today (June 30, 2022) marks last day of Pride Month of
2022. It was a weird but also enjoyable one in my opinion. I hope the
LGBTQIA+ people using this ROM on their Rosemary can say the same too.
This doesn't mean I'll drop updates of course! With the rapidly
accelarating progress of my works on OSS vendor, I assume we'll get an
open source vendor in no time! If it works fine when flashed over
existing build of Kasumi, I'll release as OTA. Otherwise, I'll need to
think some other thing for this.

Enjoy it!
                       Beru "Stella" Hinode

-----------------------------------------------------------------------

1f4191e (HEAD -> kasumi-v1, origin/kasumi-v1) rosemary/common.prop: Use HintManager for HWUI
1047c77 rosemary/overlay/RF: Don't let burn-in protection shift too far
