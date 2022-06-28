Another day, another fixup. This one shoots a good one out this time.

Maybe you remember, I once appended "Make sure you flash custom
recovery after each OTA. Otherwise you'll be left with Lineage recovery
without a working display". Say no more, it also works now! When you
check the commit though, it has quite a lot of purge possibly because
what's purged is useless.

Thanks to @woomymy for her fix and patch on this. Even though it's
hacky, it works.

Other than that, I have also attempted to fix the issue where minimum
brightness was much higher than the value we expected - It was at 21%
while resources say it has to be 10%! I tried to change the value in
system resources before realizing this, and so I still call it an
"attempt". Guess I'll still be flashbanged at nights for now.

Another sad news, the bug with in-call volume where it was at highest
value unconditionally is somehow back, I'll try my best to fix that
one as well. But unlikely to be fixed unless I go OSS vendor.

Anyway, following is a short-log for changes since last update. So
interested ones can check it out.

Enjoy!

                        Beru "Stella" Hinode

-----------------------------------------------------------------------

```
d304fd6 (HEAD -> kasumi-v1, origin/kasumi-v1) rosemary/recovery: Fix black screen on recovery
 52 files changed, 14 insertions(+), 1894 deletions(-)
b9c583c rosemary/overlay/RF: Set minimum brightness and dim much lower
 1 file changed, 2 insertions(+), 2 deletions(-)
```
