# bicubic [![experimental](http://hughsk.github.io/stability-badges/dist/experimental.svg)](http://github.com/hughsk/stability-badges) #

Bicubic interpolation - traditionally used for scaling up images or heightmaps.

## Usage ##

[![bicubic](https://nodei.co/npm/bicubic.png?mini=true)](https://nodei.co/npm/bicubic)

### `bicubic(x, y, values...)` ###

`x` and `y` are two values between 0 and 1 that determine the point of
interpolation. These are followed by a remaining *16* arguments, each of
which represent the value of a neighboring point. They're specified in
this order:

* `point(0, 0)`
* `point(0, 1)`
* `point(0, 2)`
* `point(0, 3)`
* `point(1, 0)`
* `point(1, 1)`
* `point(1, 2)`
* `point(1, 3)`
* `point(2, 0)`
* `point(2, 1)`
* `point(2, 2)`
* `point(2, 3)`
* `point(3, 0)`
* `point(3, 1)`
* `point(3, 2)`
* `point(3, 3)`

This obviously isn't the most intuitive API, so you can use
[bicubic-sample](http://github.com/hughsk/bicubic-sample) to get something
a little friendlier.

## License ##

MIT. See [LICENSE.md](http://github.com/hughsk/bicubic/blob/master/LICENSE.md) for details.
