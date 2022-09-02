# ⏱ load-control 

Control which parts of a page load, and when. Fine-grained control using the `loadindex` attribute. Framework agnostic.

Tik tok tik tok...

# `loadindex`

The API of this library is simple. Just put a `loadindex` on any element you want to control the load sequence of (how it displays into the page). Understood values are:

0 - loads in natural order.
1 - loads before anything in natural order.
n - loads before anything with loadindex n-1 or below.

And to prevent loading, use:

-1 - does not load, does not display.

In this way loadindex parallels the concepts of the global attribute [`tabindex`](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/tabindex)


