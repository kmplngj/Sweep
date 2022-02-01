# Sweep

![](/gallery/sweep2-splash.jpg)

<span>
  <a href="https://discord.gg/czXcTXbsgU">
    <img src="https://discordapp.com/api/guilds/669011382284451861/widget.png?style=shield">
  </a>
  <img src="https://img.shields.io/github/last-commit/davidphilipbarr/sweep">
</span>

## What is sweep?

Sweep is a version of the more fabulous [Ferris](https://github.com/pierrechevalier83/ferris) by [Pierre Chevalier](https://github.com/pierrechevalier83/) that uses a daughter board like a promicro, elite-c, bit-c, nice!nano etc. instead of using onboard components.

## What are the different types?

| Device | Bluetooth Support<sup>[1]</sup> | On/Off Switch | Reversible PCB | Choc V1 | Choc V2 | Choc Mini | MX & Alps | Choc Spacing<sup>[2]</sup> | Tenting<sup>[3]</sup> |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Sweep2.x          | ✔ | ✔ |   | ✔ |   |   |   | ✔ | ✔ |
| Sweep Bling MX    | ✔ | ✔ | ✔ |   |   |   | ⚠<sup>[4]</sup> |   | ✔ |
| Sweep High        | ✔ | ✔ |   | ✔ | ✔ |   | ✔ |   | ✔ |
| Sweep Half Swept  | ✔ | ✔ | ✔ | ✔ |   |   |   | ✔ | ✔ |
| Sweep Compact Low | ✔ |   | ✔ |   |   | ✔ |   | ✔ |   |

*<sup>[1]</sup> It simply means that it supports the nice!nano. An on/off switch is recommended for bluetooth*  
*<sup>[2]</sup> Choc spaced boards have the switches in a tighter grid. This provides a better final look but is only compatible with some choc keycaps (e.g. MBK)*  
*<sup>[3]</sup> Supports splitkb's [tenting puck](https://splitkb.com/products/tenting-puck?_pos=1&_psq=tenting%20&_ss=e&_v=1.0)*  
*<sup>[4]</sup> MX + kailh hotswap ONLY. Alps are NOT supported*  


* Sweep2 - Recommended Choc v1 board with all the features.
* Sweep Bling MX - An MX only Sweep that features Kailh's hotswap sockets and a stacked case.
* Sweep High - Same as the Sweep2 but trades choc spacing for compatibility with more switches and keycaps.
* Sweep Half Swept - Half of a Sweep2 with double pro-micro footprint (letting you avoid having one daughter-board flipped upside-down)
* Sweep Compact Low - The only version that supports Choc minis.

## Components list

To build and use a Sweep you will need:

* 1x PCB Kit
* 2x promicro compatible boards or 2 nice!nanos.
* 34 switches of a compatible type (refer to the compatibility table)
* 34 keycaps
* 2x reset switches (optional; [B3U-1000P(M)](https://github.com/davidphilipbarr/Sweep/issues/20))
* Some little rubber feet/bumpers
* 2x power switches (optional if supported; MSK 12C02)
* 1x TRRS (not TRS!) cable (wired build only)
* 2x TRRS Jack [PJ-320A] (wired build only)
* 1 USB Cable (depends on your micro-controller choice)

## How do I make this thing?

<a href="https://www.youtube.com/watch?v=fBPu7AyDtkM" target="_blank">
  <img src="https://gist.githubusercontent.com/duckyb/337340baa1f0c8bcc06fef7b3b57242b/raw/97e6e0748dd1b8a3fb54fac0a88e84e6b6e0e10a/build-guide-button.svg" height="44">
</a>

## Firmware

The firmware can be found [with the Ferris  firmware as part of QMK](https://github.com/qmk/qmk_firmware/tree/master/keyboards/ferris/sweep).

Firmware for zmk and bluemicro_ble is called ["Cradio"](https://zmk.dev/docs/hardware/).

## Keyboard Layout

Here is the link to the Sweep layout for the [Keyboard Layout Editor](http://www.keyboard-layout-editor.com/##@@_r:25&rx:1&ry:1&y:-1.1&x:2&c=%23555657&t=%23ffffff%0A%23e5ff47%0A%23fa00ff%0A%2300d1ff%3B&=E%0AF8%0A*%0A8%3B&@_y:-0.6499999999999999&x:1%3B&=W%0AF7%0A%2F&%0A7&_x:1%3B&=R%0AF9%0A(%0A9%3B&@_y:-0.75%3B&=Q%0AF12%0A%7B%0A%5B%3B&@_y:-0.9&x:4%3B&=T%0APtSc%0A%7D%0A%5D%3B&@_y:-0.7000000000000001&x:2%3B&=D%0AF5%0A%25%0A5%0ALCTRL%3B&@_y:-0.6499999999999999&x:1%3B&=S%0AF4%0A$%0A4%0ALALT&_x:1&n:true%3B&=F%0AF6%0A%5E%0A6%0ALSHFT%3B&@_y:-0.75%3B&=A%0AF11%0A%2F:%0A%2F%3B%0ASuper%3B&@_y:-0.8999999999999999&x:4%3B&=G%0ASLck%0A+%0A%2F=%3B&@_y:-0.7000000000000002&x:2%3B&=C%0AF2%0A%2F@%0A2%3B&@_y:-0.6499999999999999&x:1%3B&=X%0AF1%0A!%0A1&_x:1%3B&=V%0AF3%0A%23%0A3%3B&@_y:-0.75%3B&=Z%0AF10%0A~%0A%60%3B&@_y:-0.8999999999999999&x:4%3B&=B%0ABreak%0A%7C%0A%5C%3B&@_r:30&rx:0&ry:0.25&y:2.5&x:4.75&t=%23ffffff%0A%0A%23fa00ff%0A%2300d1ff%0A%23ff0000&a:0%3B&=⭾%0A%0A)%0A0%0ANav%3B&@_r:35&rx:1&ry:0&y:4&x:-1&c=%23cccccc&t=%23000000&a:7%3B&=%3B&@_r:45&rx:1.25&ry:0.6&y:1.4499999999999997&x:5.4&c=%23555657&t=%23ffffff%0A%0A%23fa00ff%0A%2300d1ff%0A%0A%2342ff00&a:0%3B&=↵%0A%0A%2F_%0A-%0A%0AMedia%3B&@_r:-35&rx:9.5&ry:5&y:-0.5350000000000001&x:-2.5&t=%23ffffff%0A%0A%0A%23ff0000%0A%2300d1ff%0A%23e5ff47%3B&=␣%0A%0A%0AEsc%0ANum%0AFn%3B&@_r:-25&ry:3.75&y:-2.9850000000000003&x:-0.5&t=%23ffffff&a:4%3B&=I%3B&@_y:-0.6499999999999999&x:-1.5%3B&=U&_x:1%3B&=O%3B&@_y:-0.75&x:1.5&t=%23ffffff%0A%0A%2342ff00%3B&=P%0A%0ABT✕%3B&@_y:-0.8999999999999999&x:-2.5&t=%23ffffff%3B&=Y%3B&@_y:-0.7000000000000002&x:-0.5&t=%23ffffff%0A%0A%0A%23ff0000%3B&=K%0A%0A%0A🡇%0ARCTRL%3B&@_y:-0.6499999999999999&x:-1.5&n:true%3B&=J%0A%0A%0A🡄%0ARSHFT&_x:1%3B&=L%0A%0A%0A🡅%0ALALT%3B&@_y:-0.75&x:1.5%3B&=%2F%3B%0A%0A%0A🡆%0ASuper%3B&@_y:-0.8999999999999999&x:-2.5&t=%23ffffff%3B&=H%3B&@_y:-0.7000000000000002&x:-0.5&t=%23ffffff%0A%0A%2342ff00%0A%23ff0000%3B&=,%0A%0ABT3%0APgDn%3B&@_y:-0.6499999999999999&x:-1.5%3B&=M%0A%0ABT2%0AHome&_x:1%3B&=.%0A%0ABT4%0APgUp%3B&@_y:-0.7500000000000004&x:1.5%3B&=%2F%2F%0A%0ABT5%0AEnd%3B&@_y:-0.9000000000000004&x:-2.5&t=%23ffffff%0A%0A%2342ff00%3B&=N%0A%0ABT1%3B&@_r:-20&rx:11.5&ry:4&y:0.11500000000000021&x:-3.5&t=%23ffffff%0A%0A%0A%23ff0000%0A%23e5ff47%0A%23fa00ff&a:0%3B&=⌫%0A%0A%0A⌦%0AFn%0ASym).

[Here is a variante](http://www.keyboard-layout-editor.com/##@@_r:25&rx:1&ry:1&y:-1.1&x:2&c=%23ffffff%3B&=E%0AF8%0A*%0A8%3B&@_y:-0.65&x:1&t=%2300000%3B&=W%0AF7%0A%2F&%0A7&_x:1&t=%23000000%3B&=R%0AF9%0A(%0A9%3B&@_y:-0.75%3B&=Q%0AF12%0A%7B%0A%5B%3B&@_y:-0.9&x:4&t=%2300000%3B&=T%0APtSc%0A%7D%0A%5D%3B&@_y:-0.7&x:2&t=%23000000%3B&=D%0AF5%0A%25%0A5%0ALCTRL%3B&@_y:-0.6500000000000001&x:1%3B&=S%0AF4%0A$%0A4%0ALALT&_x:1&n:true%3B&=F%0AF6%0A%5E%0A6%0ALSHFT%3B&@_y:-0.75%3B&=A%0AF11%0A%2F:%0A%2F%3B%0ASuper%3B&@_y:-0.8999999999999999&x:4%3B&=G%0ASLck%0A+%0A%2F=%3B&@_y:-0.7&x:2%3B&=C%0AF2%0A%2F@%0A2%3B&@_y:-0.6499999999999999&x:1%3B&=X%0AF1%0A!%0A1&_x:1%3B&=V%0AF3%0A%23%0A3%3B&@_y:-0.75%3B&=Z%0AF10%0A~%0A%60%3B&@_y:-0.8999999999999999&x:4%3B&=B%0ABreak%0A%7C%0A%5C%3B&@_r:30&rx:0&ry:0.25&y:2.5&x:4.75&a:0%3B&=⭾%0A%0A)%0A0%0ANav%3B&@_r:35&rx:1&ry:0&y:4&x:-1&c=%23cccccc&a:7%3B&=%3B&@_r:45&rx:1.25&ry:0.6&y:1.4499999999999997&x:5.4&c=%23ffffff&a:0%3B&=↵%0A%0A%2F_%0A-%0A%0AMedia%3B&@_r:-35&rx:9.5&ry:5&y:-0.5350000000000001&x:-2.5%3B&=␣%0A%0A%0AEsc%0ANum%0AFn%3B&@_r:-25&ry:3.75&y:-2.985&x:-0.5&a:4%3B&=I%3B&@_y:-0.6499999999999999&x:-1.5%3B&=U&_x:1%3B&=O%3B&@_y:-0.75&x:1.5%3B&=P%0A%0ABT✕%3B&@_y:-0.8999999999999999&x:-2.5%3B&=Y%3B&@_y:-0.7&x:-0.5%3B&=K%0A%0A%0A🡇%0ARCTRL%3B&@_y:-0.6499999999999999&x:-1.5&n:true%3B&=J%0A%0A%0A🡄%0ARSHFT&_x:1%3B&=L%0A%0A%0A🡅%0ALALT%3B&@_y:-0.75&x:1.5%3B&=%2F%3B%0A%0A%0A🡆%0ASuper%3B&@_y:-0.8999999999999999&x:-2.5%3B&=H%3B&@_y:-0.7000000000000002&x:-0.5%3B&=,%0A%0ABT3%0APgDn%3B&@_y:-0.6499999999999999&x:-1.5%3B&=M%0A%0ABT2%0AHome&_x:1%3B&=.%0A%0ABT4%0APgUp%3B&@_y:-0.75&x:1.5&t=%2300000%3B&=%2F%2F%0A%0ABT5%0AEnd%3B&@_y:-0.8999999999999999&x:-2.5%3B&=N%0A%0ABT1%3B&@_r:-20&rx:11.5&ry:4&y:0.11500000000000021&x:-3.5&t=%23000000&a:0%3B&=⌫%0A%0A%0A⌦%0AFn%0ASym) that is printable on a monochrome printer. 

Default is [Miryoku](https://github.com/manna-harbour/miryoku) inspired, the default is there to be replaced. You could use this as a base to create and save your own layout version.

## Who made this?

* [Pierre Chevalier](https://github.com/pierrechevalier83)
* [David Barr](https://github.com/davidphilipbarr)
* [Ibnu Daru Aji](https://github.com/ibnuda/)
* [Duccio](https://github.com/duckyb)

