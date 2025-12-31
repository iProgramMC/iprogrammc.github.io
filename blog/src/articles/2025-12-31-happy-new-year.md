TITLE:Happy New Year 2026!
DESCRIPTION:iProgramInCpp wishes you a happy new year and talks about what he did in 2025.

# Happy New Year 2026!

This year has been even more chaotic and eventful than the last, both in the world as well as in my life.
I got to know a few more people in real life, and I got to see a lot of stuff I hadn't seen before.

Let's talk about what I achieved this year:

## Discord on Windows NT 3.x and 9x

I talk more about it in [one of my previous articles](2025-03-30-discord-on-nt-3-1.html).  I got DM working on
Windows 9x in early February, and that attracted the [attention](https://www.tomshardware.com/software/windows/modern-discord-hacked-into-windows-95-and-98-slimmed-down-version-keeps-core-functionality-intact)
of [several](https://hackaday.com/2025/06/17/how-discord-was-ported-to-windows-95-and-nt-3-1/)
[news](https://www.techspot.com/news/106624-custom-discord-client-brings-modern-chat-windows-95.html)
[publications](https://www.pcgamer.com/games/this-third-party-retro-ui-for-discord-looks-like-and-even-runs-on-windows-98/),
and [even MattKC himself](https://www.youtube.com/watch?v=wxdn30G2LE8)!  That last YouTube video was edited by good
friend [Wam](https://wamwoowam.co.uk), and he probably nudged Matt to do it, so thank you so much!

One more thing, Discord now runs on Pentium processors, thanks to a custom cross-compiler I built, and overall
the setup is a lot less janky than it used to be.

## Boron

[Link to the operating system project](https://github.com/iProgramMC/Boron)

My operating system project has evolved significantly from last time.  It now looks like this:

![Boron showing a simple mlibc application running](images/boron-userspace.png)

Everything you see here is drawn in user mode. The frame is inspired by NeXTSTEP, however I will probably change
it in the future. The featured program is a simple one trying the new-fangled `fork()` (really, `OSForkProcess()`)
implementation.

Next year I want to work on getting bash and some coreutils running inside of Boron, and then start working on a
window system. I had been waiting for this moment since 2023 and it feels ever closer as time goes on.

Also, in October I started porting the kernel to i386, for fun. This port targets legacy hardware (for example, i486),
but currently only runs on Pentium Pro and higher, because I don't have a cross-compiler for the 486 yet.

In late December I challenged myself to try and port Boron to armv6, and to run on an iPhone 3G. However, unfortunately,
I couldn't achieve this goal. I *did* manage to get the kernel running inside QEMU on a versatilepb board, and as of
now I am writing the HAL for this port. I haven't decided how the boot process will go yet (whether through a restore
ramdisk and pwned DFU, or through OpeniBoot).

Nevertheless, I've made tremendous progress on this operating system. While it's not yet as good as it could be, I'm
certain that 2026 will be the year the OS finally gets "good".

Some random goals I want to achieve with this OS:
- Running `bash` + `coreutils`
- Running `gcc`
- Running `python3` and `nasm`
- Self-hosting (what I mentioned above, as well as `xorriso`, is basically what's needed for that)
- Writing my own window manager
- NanoShell compatibility (for the love of the game)

## My iPhone Collection

Throughout late 2025 (starting June 19th and ending on December 20th with my last purchase), I have built up
a pretty sizable collection of iPhones. I will only go into detail about the phones that work.

- iPhone 3G (first): I bought this one in mid-June. According to settings, it came with iOS 3.1.3, but I
  have my doubts, because it has several iOS 4 features such as wallpaper, icon groups, dock, and the iOS 4
  Voice Memos icon. However, apparently they have an "iOS 3 Wallpaper" tweak installed from Cydia, so I don't
  know for sure.

- iPhone 3G (second): I bought this one like 2 weeks later. It was in bad condition, huge crack through the touch
  digitizer splitting it in half, and messed up back. However, the screen was in great condition. So I ended
  up mixing the LCD from this 3G and putting it with the touch screen of the first one, and made a working
  phone. For a while, I kept the first iPhone's motherboard, but it didn't accept connecting to any Wi-Fi
  networks whatsoever so I decided to try and restore the second board. It initially showed the "Connect to
  iTunes" logo, but I had learned of Legacy iOS Kit and managed to revive that board. It's now happily running
  iOS 3.1.3, and has been my main workhorse in developing Purplecord.

- iPhone 3G (third): This one I bought in early October. It initially had a problem where the NAND wasn't responding,
  but I waited a good while and tried again. I managed to get the phone in working condition and it now runs iOS 2.0.
  It's nothing more than a novelty, though.

- iPhone 3G (fourth): Bought this one in mid-November. It came with iOS 4.2.1, and it was chock full of apps of
  French origin. I backed them all up. For anyone curious, here's the link: https://mega.nz/folder/KAtiBKpZ#vc-4YoBQgcV7R1fYh7mohw
  (If any French app developer has any problems with this link I'll remove it)

- iPhone 4 (black): Early October. Has been my second testing workhorse. It's running iOS 7.0 right now.

- iPhone 4 (white): Early November, I think? It's carrier locked, so I couldn't activate it legitimately on iOS
  7. I had to hacktivate it on iOS 6.

- iPhone 4 (second black): Probably around early November too. It doesn't do much, but it is activated on iOS 7.1.2
  and in good condition.

- iPhone 3GS: Early October. I use this one from time to time whenever I feel the need to use iOS 6.

- iPod touch 2nd Generation: Early November, I believe. I once had a problem on iOS 4.2.1 where the NAND was temporarily
  messed up. But after 2 years it seems to have been fine. I restored it to iOS 3.1.3 and now it's stable. But I will
  be careful with it as I don't want to lose it permanently. This one cost the most amount of money from the other
  devices but I feel ripped off.

- iPod touch 3rd Generation: Mid-December. It came with iOS 5.1.1. Had some woman's data on it. Not much to say.

- iPad 3G 1st Generation: Mid-December. I hesitated to buy this but I decided to. When I received it, its battery was
  completely dead and was in a constant boot loop. I hacked up an old broken phone and used it to bypass the charging
  circuit of the iPad, and that somehow revived the tablet. It came mostly wiped, but was set up and activated in
  Italian on iOS 5.1.1.

I have a bunch of other phones, but they're either iCloud-locked, have cracked digitizers/LCDs, or are missing batteries,
so they're currently unusable.

## Celeste NES

I released the demo, but haven't done too much work after that. I've worked on Chapter 3 for a little bit, but it's nowhere
near complete.  And honestly I don't see myself working on this project often in the future.

## My Celeste Save File

This year, I've played a *lot* of [Celeste](https://celestegame.com). And honestly, I can't recommend it enough. It's an
awesome game. But damn is it frustrating.

Anyway, this year I achieved a total of 200 Strawberries! (175 Red Strawberries, one Moon Berry, and 24 Golden Strawberries)
That's a *really* big number.  I started the year of 2025 with 193 Strawberries. Then I collected the followingGolden berries,
in this order:

- Core A-Side
- Celestial Resort B-Side
- Mirror Temple B-Side
- The Summit A-Side
- Golden Ridge B-Side
- Reflection B-Side
- The Summit B-Side

In addition to that, I have a record of 28 deaths in Core B-Side, and 32 deaths in Farewell.

Maybe I'll get 202 in 2026, who knows? I can't guarantee it though, this game is *no joke*.

## Conclusion

The amount of work I've done this year has truly surpassed my previous years. I now have a job, driving license, and I'm
evolving as an adult. I don't know what I'll be working on next, but we'll see!

Maybe I'll come back to some of my earlier projects (like Gamma64) for shits and giggles.

**Happy new year, everyone! Enjoy the rest of the holidays!**

Thank you so much for reading this (and following my work). I really appreciate it.
