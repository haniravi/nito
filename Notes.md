# Notes

## General notes

It would be nice to have a split keyboard. Previously I thought that a TKL keuboard would be nice, but while fiddling with possible layout, it turned out TKL has too many keys. A 60%/65% keyboard however fits the desired UX just right.

It would be nice to have ****MOD**** keys, kind of like in [vim](vim.org). ****MOD**** key basically switches between layers, just like **CTRL**, **ALT**, **SHIFT** and so on. Each layer allows to encode a desired layout and behaviour.

The CAPSLOCK key is not needed. It could serve as an ESC key.

I rarely use the whole length of SPACE key. Having a SPACE key on left handside should probably be enough. The right handside SPACE could serve as a RETURN key.

Another thing I noticed is I almost never use the right shift key on my current (full)keyboards.

**MOD** keys can be sticky and not-sticky, not sure which to use yet.

[This](qibord_layout.json) is the layout file (at least the draft of it).

## Layers

After some tests (w/o the kwyboard) I decided that 4 layers will be enough.

Those layers are presented below

### Key legend

![Layer toggle key](layers/layer_toggle_key_small.jpg) is the key responsible for switching to the specified layer. In this particular image, it will switch to [layer 1](#numpad-and-the-rest-of-the-symbols-layer-layer-1).

![Next non-transparent key](layers/next_non_transparent_key_small.jpg) means that if the key has no bindings on current layer, it will act as the first next *non-transparent* key on layers below. This means that the lower-leftmost key on [layer 2](#text-navigation-layer-layer-2) will act as **Left Ctrl**. Generally, _all control keys_ are set on [layer 1](#default-layer) and referenced like so from other layers.

### Default Layer

By default layer, I mean the layer that is active when no layer toggle keys are pressed. It contains the alphas and the _unshifted_ symbols. As you can see, the numerals and _shifted_ keys are not here. The **SHIFT** key on this layer is used only to capitalize letters. This is the only responsibility of **SHIFT** key on _Qibord_.

Other uses of the **SHIFT** key were bound to layer keys. You may notice that on this layer, only the opening brackets are present. Their counterparts are situated on the next layer.

Same goes for the numerals.

Below is a possible layout of the layer.
![Default layer](layers/default_layout.jpg)

### Numpad and the rest of the symbols layer (layer 1)

This layer contains the digits and missing symbols from the default layer. Again, I dont want to use the **SHIFT** key for switching between the symbols. I also do not like typing the numbers via the horizontal keys, it's too much movement. One more thing I want to try, is a mapping of symbols different from **SHIFT** one. It seems to me that it is more intuitive to map the opening and closing braces to the same key and switch via a ****MOD**** key.

Below is a possible layout of the layer.
![Numpad and Symbold layer](layers/numpad_and_symbols.jpg)

### Text navigation layer (layer 2)

Below is a possible layout of the layer.
![Text navigation layer](layers/text_navigation.jpg)

### **Fn** and Media layer (layer 3)

Below is a possible layout of the layer.
![**Fn** and Media layer](layers/fn_keys_and_media.jpg)

## Hardware

### Current choice

I decided to go with [Nyquist/Levinson (Rev. 3)](https://keeb.io/collections/split-keyboard-parts/products/nyquist-keyboard) - an ortholinear 60%/40% split keyboard. I will be using all 60% of it - two 5x6 plates.

### Older considerations

The boards below have too much keys.

[KBO-5000](https://keeb.io/collections/frontpage/products/kbo-5000-split-staggered-80-keyboard) 80% keyboard seems to be a nice place to start.

[BFO-9000](https://keeb.io/collections/frontpage/products/bfo-9000-keyboard-customizable-full-size-split-ortholinear) is another option but I do not see how to assemble it yet.

----------

#### Misc

It would be nice to keep the **MOD** keys far from each other, so I wont press a wrong key by mistake.

It seems that mapping opening and closing brackets to the same key with **MOD** switch requires less space keys and the same amout of strokes.
Also to me it is more intuitive.
