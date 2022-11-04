ALPS 60% keyboard PCB
=====================
This supports 60% AEK and other layouts and fits into GH60/Poker X compatible cases. See this page for other infos.

https://geekhack.org/index.php?topic=91843.0


Revisions
---------
Rev.A   2015/03
Rev.B   2015/05     ISO Enter fix
Rev.C   2015/10     Silk fix: position of K70, K40 and value of resistor:10K -> 1K
                    Capslock for Cherry Stepped 1.25u
Rev.D   2016/04     Fix Xtal foot print and value of R and C
Rev.E   2016/08     Retouch USB connector footprint and silks
Rev.F   2017/08     Add breakout for unused pins(PC4, PC6, PC7)
Rev.J   2019/09     Update footprints and remove R for HWB
Rev.K   2022/11     Replace Mini-B with USB-C and remove KBP V60 support


TODO
----
Footprint library
    Centroid: Diode and capacitor footprint
    Pin1 is cathode or capacitor-positive. Pin1 is left for two pin devices like resitor and caps.
    Pin1 is on upper left for many pin device like DIP, QFP, SOT...
    http://pcbget.ru/Files/Standarts/IPC_7351.pdf
    http://www.screamingcircuits.com/Home/HowItWorks
    http://i.screamingcircuits.com/docs/understanding-the-centroid-file-r2-2.pdf
Schematic:
    reversed pins of LED: create new LED component
Silk fix:                                           DONE 10/09
    placement of K70, K40
    value of resistor:10K -> 1K
Capslock for Cherry Stepped 1.25u:                  DONE 10/09
    Someone may use Cherry keycaps with stem adapters.
    never seen 1.25u stepped Capslock for Alps, normally 1.5u stepped or 1.75u(no stepped) for Alps

ISP pads:
Support for infinity bottom row: 1.5, 1, 1, 1.5:    DONE 03/05
Thumb keys, split space bar:                        near future
Trackpoint support: mount holes and IO pins:        Future revision
Bluetooth support:                                  Future revision

USB connector should be shifted to outside by 0.3-0.5mm. 04/05

ISO Enter Support:
    ISO Enter key can be used in Rev.B and later revision. The PCB supports three mount positions, 1u, 1.25u and 1.5u. See pictures and figure below. Matias has 1.25u mount, Dell and Alps have 1.5u mount and ISO Enter with 1u mount is not confirmed its existence yet. By the way, Cherry ISO key is also located in middle of 1.25u as Matias does.

    keycap from Matias
        https://geekhack.org/index.php?topic=69740.msg1760105#msg1760105
        http://i.imgur.com/tiPWImU.png
    keycap from NEC Rakuraku keyboard(Alps)
        https://geekhack.org/index.php?topic=69740.msg1760805#msg1760805
        http://i.imgur.com/YKIbKlrl.jpg
    keycap from Dell AT102W
        https://geekhack.org/index.php?topic=69740.msg1761095#msg1761095
        https://geekhack.org/index.php?action=dlattach;topic=69740.0;attach=101849;image


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

TODO:
Poker3/Pok3r case
https://massdrop-s3.imgix.net/product-images/MD-6955_20150414182153_3159611692efb865.jpg


Pics and Resources
------------------
Apple Extended Keyboard & II:
    http://i.imgur.com/mB5pcJy.jpg
    AEK ISO is not standard, weirdly shfted to right and not supported.
    http://www.finestcomputers.co.uk/FinC/Apple/hardware/ExtendedKeyboard-II/No.3/EK2-1.JPG

Dutch Apple Extended Keyboard with different spacebar stab(2018/05)
    https://i.imgur.com/I1DEexi.jpg
    https://geekhack.org/index.php?topic=69740.msg2604163#msg2604163

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
