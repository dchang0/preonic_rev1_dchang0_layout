# preonic_rev1_dchang0_layout

Hi, everyone!

This is my custom QMK layout/keymap for the awesome OLKB Preonic Rev. 1 or Rev. 2 ortholinear keyboard. You can get the official QMK firmware here:

https://github.com/qmk/qmk_firmware

Put the folder `dchang0_rev1` with all its contents inside the `qmk_firmware/keyboards/preonic/keymaps` folder in your QMK source code folder tree, then build and flash it as normal with the command:

```
make preonic/rev1:dchang0_rev1:dfu
```

Remember to push the reset button on the bottom of the Preonic for the flashing to start before the DFU utility times out.

You can ALMOST use this layout for the Rev. 3, but the Rev. 3 has a need for more RGB LED backlight controller keys on the Adjust layer.

For Rev. 3 the flashing command is slightly different. If you want to use this layout, it will be:

```
make preonic/rev3:dchang0_rev1:dfu-util
```

-----

Here's the theory/impetus/backstory behind this custom layout.

I'm a LINUX and Windows programmer, and I got a light case of carpal tunnel several years ago. You're probably wondering: 'A "light" case? How do you get a "light" case of carpal tunnel?' I walked right up to the edge, recognized I was about to cross the point of no return, and decided I had to make drastic changes to my workstation ergonomics. First, I had to get away from the standard ANSI staggered QWERTY layout.

This included researching/testing Dvorak layout and ortholinear and split ortholinear keyboards and mechanical keyswitches like my life depended on it (it does, because I lost a customer from not being able to keep up with their deadlines due to my injury--keep it up and I wouldn't be able to eat), and eventually after lots of trial and error, I ended up with the Preonic Rev. 1. hardware with lightweight Red (45gf) or Yellow (50gf) linear mechanical keyswitches. 

I had learned from the Matteo WhiteFox "True Fox" layout that just bringing in the Backspace key closer to the home row resulted in a real feeling of relief after hours of typing. Any time I used a True Fox layout and then sat down at someone else's standard keyboard, I would hit the backslash/pipe key thinking it was Backspace. My hands had expressed a clear preference (thank you, Matteo!). So I knew I needed to relocate at least the Backspace key.

Most staggered layouts with keys greater than 1U are just not customizable when it comes to moving important keys like Enter, Backspace, ESC, Tab and Space. 1U ortholinears are one of the few keyboards where you can truly put any key you want anywhere. I liked having the number row of the Preonic even though it does require a bit of stretching to reach; the convenience outweighs the slight pain. As for why I went with a non-split ortholinear, I also game occasionally, and a one-piece keyboard is eaiser to operate one-handed, with the other hand on the mouse.

Once I got the Preonic, I started testing/trying out many of the layouts that come with the official QMK firmware. None of them were just right for me, so I developed this custom layout from the default layout for these reasons:

a) I didn't like the lack of a Right Shift on most Preonic layouts. Its absence makes typing capitals on the left side of the keyboard tedious. Not having a CAPSLOCK is a pain too, but there's no room for one. I had to add CAPSLOCK to a layer (see below).

b) I can tell by the shiny spot worn into my space bar that I really only need a 1U spacebar, not 2U and certainly not 2x 2U.

c) It's painful to have to twist the wrists to reach for the ESC (vim), Backspace, and Enter keys so frequently, so I moved the Backspace and Enter keys down to the left and right of the Lower and Raise keys, respectively. They are operated with the thumbs, without moving the wrists or moving the fingers from the home row. I can tell my hands really like the Enter key being operated by the right thumb. My hands are less happy about the Backspace key being operated by the left thumb--the problem is that the Alt key is right next to it. Sometimes I overshoot the Backspace and hit Alt, which usually opens the application's menu bar in Windows. It requires a bit more precision than I have in my left hand (I am very strongly right-handed). But, if I focus on typing more accurately, then Backspace is used much less often.

You can probably tell I swapped GUI and Alt--that's because overshooting Backspace and hitting GUI and accidentally opening the Start menu is a lot more annoying than hitting Alt.

BTW, I mapped Delete = Lower + Backspace OR Raise + Backspace. It works well.

d) I used to think I almost never used CAPSLOCK and that it is superfluous, but after losing it, I realized just how useful it is and that I use it quite often. So I tried mapping it to Lower + Left Shift, but that turned out to be awful because Lower + Left Shift is used in other three-key combos. So I moved it to Raise + Right Shift. It feels good there.

Shortcomings of this layout:

Really, these are shortcomings of most 60-key or smaller keyboards.

e) For a programmer, it is really annoying to not have the square brackets and curly braces on the base layer. I am thinking hard about sacrificing some other keys to get the square brackets, but there is nothing to sacrifice. Maybe I should get a 13 x 5 = 65 1U key ortholinear? But then I'm reaching too far from the home row again, and the brackets wouldn't be right next to each other anyway--they'd be one above the other... It's a conundrum.

f) Also, combining + and = with - and _ is annoying. I have to use Lower + Shift to get +. This too would be solved by a 13th column on the right edge.

That said, the Preonic with this layout did pull me back from the brink of full-on carpal tunnel, so I may just have to suck it up and deal with these two annoyances.


I hope you enjoy using my custom layout or drawing inspiration from it to design your own!
