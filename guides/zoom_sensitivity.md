# Editing zoom scroll sensitivity

#### Corresponding branch: [smoother_scroll](https://github.com/Juliapixel/M3da/tree/smoother_scroll)

#### List of [changes](https://github.com/Juliapixel/M3da/compare/master...smoother_scroll)

-----

The file [`M3da/M3daview.cpp`](/M3da/M3daView.cpp) has all the keystroke handling logic. in it, the class method `CM3daView::OnMouseWheel` controls the renderer's display scale by adding the original scale, multiplied by a predefined value `dSR`, to itself. The smaller `dSR` is, the smaller the increments in zoom are, with negative values inverting the zoom direction (scroll down becomes zoom-in, scroll up becomes zoom-out).

`dSR` is defined on [line 589](/M3da/M3daView.cpp#L589).
