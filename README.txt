ALPS 60% keyboard PCB
=====================
Primary goal is to support 60% cut AEK(Apple Extended Keyboard) layout and fits into Poker X cmpatible cases.


Revisions
---------
Rev.A   2015/03
Rev.B   2015/05     ISO Enter fix


Ideas
-----
### LED ###
Backlight won't support. Indicators may be needed for debug.
LED footprint for ALPS Green?

### PCB mount plate: ###
1.6mm PCB will be OK for switch plate.
SMD LED? WS2812? Matias style underside LED?

### TrackPoint ###
ATMega32u2 has no spare pins for TrackPoint three buttons and signals.


TODO
----
ISP pads:
Support for infinity bottom row: 1.5, 1, 1, 1.5:    DONE 03/05
Thumb keys, split space bar:                        near future
Trackpoint support: mount holes and IO pins:        Future revision
Bluetooth support:                                  Future revision

USB connector should be shifted to outside by 0.3-0.5mm. 04/05

ISO Enter Fix:
    keycap from Matias doesn't work with Rev.A
        https://geekhack.org/index.php?topic=69740.msg1760105#msg1760105
    keycap from NEC Rakuraku keyboard doesn't work too
        https://geekhack.org/index.php?topic=69740.msg1760805#msg1760805

    Matias mount is located at middle of 1.25u while 1.5u on NEC keycap(Alps?).
    ISO Enter key position of Rev.A is middle of 1u but such Enter key doesn't exist perhapse.

       ------- -------
      |       |       |
      |   +   |   +   | 1u
      |       |   |   |
       ------- -------
            |     |   |
            |    +|   | 1.25u
            |    ||   |
            `---------'
          |      ||   |
          |     +||   | 1.5u
          |     |||   |
          `-----------'
          .-----------, 1.5u
          |     |||   |
          |     |||   |
           `    +++   |
            |         |
            |         |
            `---------' 1.25u



Support Layouts
---------------
Hopefully supports AEK, KBP V60, Omnikey and Dell layouts. AEK ISO layout is not supported due to its anormaly. See below link.

Top right:
    \, `        (HHKB style)
    Backspace   (US)

Right shift:
    RShift, Fn  (HHKB/Omnikey style)
    RShift      (US)

Bottom row:
    1.5, 1.25, 1.5,     space 6.5,  1.5, 1.25, 1.5          (AEK)
    1.5, 1, 1.5,        space 7,    1.5, 1, 1.5             (101key,103key)
    1.25, 1.25, 1.25,   space 6.25, 1.25, 1.25, 1.25, 1.25  (V60, 104key, Infinity Standard)
    1.5, 1, 1.5,        space 6,    1.5, 1, 1, 1.5          (Infinity Hacker)

ISO:
    ISO Enter key
    ISO LShift

Space bar:
    7.0u                                                    (AEK, 101key, 103key)
    6.375u                                                  (V60, 104key, Infinity Standard)
    6.5u                                                    (Infinity Hacker)

Caps lock:
    0.75u(3/8)                                              (Non Stepped)
    0.25u(2/8)                                              (Dell/SGI Stepped)
    0.125u(1/8)                                             (Cherry Stepped)

(key unit; Top row: Esc[0u], 1[1u], ... 7[7u], ...)


Support Cases
-------------
Poker X case and its compatibles.
Also V60 case are supported hopefully with ballpark figure from pics.


Pics and Resources
------------------
Apple Extended Keyboard & II:
    http://i.imgur.com/mB5pcJy.jpg
    AEK ISO is not standard, weirdly shfted to right and not supported.
    http://www.finestcomputers.co.uk/FinC/Apple/hardware/ExtendedKeyboard-II/No.3/EK2-1.JPG

KBParadise V60 with Matias:
    https://geekhack.org/index.php?topic=57386.30
    http://deskthority.net/review-f45/kbp-v60-matias-click-and-matias-quiet-click-keyboards-t9502.html
    PCB:    http://i.imgur.com/Mj51unC.jpg
    PCB:    http://www.hardcoreware.net/wordpress/wp-content/uploads/2014/06/kbp-v60-mini-review-pcb.jpg
    Case:   http://i.imgur.com/WiYtefc.jpg
    On their Facebook they said:
    we can screw V60 plate on 4 holes of Poker2/Pure Pro case. Basicly , V60 can fit in Poker 2 case. But V60 has 6 dip switch , Poker 2 only has 4 dip switch. If the back side hole space not enough , the plate touch , not balance.
Poker 2 can not fit in V60 case. Because V60 case is a little smaller than Poker 2.

Northgate Omnikey 101key:
    http://cdn.overclock.net/1/15/900x900px-LL-15fea91e_29fpe1c.jpeg
    http://www.overclock.net/t/538389/official-mechanical-keyboard-club-because-saving-money-is-boring/12140#post_19494881
    http://sandy55.fc2web.com/keyboard/omnikeyultra.html

Dell/SGI 101    Spacebar pos:7u
    http://deskthority.net/w/images/9/96/Sgi_granite_203.jpg

Dell 101W(104key with Windows key)  Spacebar pos 6.375u
    https://geekhack.org/index.php?topic=50993.msg1126977#msg1126977
    https://geekhack.org/index.php?action=dlattach;topic=50993.0;attach=45171;image

Matias switch custom keyboard:
    https://geekhack.org/index.php?topic=49920.msg1083821#msg1083821
    https://geekhack.org/index.php?topic=46060.0

Face U replica PCB(Cherry)
    http://imgur.com/a/StdLF

Nerd 60 PCB(Cherry)
    https://geekhack.org/index.php?topic=63507.0
    https://geekhack.org/index.php?topic=63507.0

Infinity PCB(Alps/Cherry)
    https://github.com/kiibohd/pcb
    https://d3jqoivu6qpygv.cloudfront.net/img_site/articles/keyboard/massdrop-infinity-circuit.jpg

Duckmini V2 PCB(Alps/Cherry)
    https://geekhack.org/index.php?topic=46060.msg1065980#msg1065980

Some case has extra standoffs
    https://geekhack.org/index.php?topic=50580
    https://geekhack.org/index.php?action=dlattach;topic=50580.0;attach=56770;image


Other Alps SKCM keyboards
    http://deskthority.net/wiki/Category:Keyboards_with_Alps_SKCL/SKCM_switches

ISO Enter(Matias: 1.25u center/Alps: 1.5u center)
    https://geekhack.org/index.php?topic=69740.msg1760105#msg1760105
    https://geekhack.org/index.php?topic=69740.msg1760805#msg1760805
    http://auctions.c.yimg.jp/images.auctions.yahoo.co.jp/image/ra118/users/4/5/3/6/kanami55bros-img591x600-1425099861y5vvwi23067.jpg
