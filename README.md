# CSS Box Shadow

- Css box shadow allows you to add shadow around an element in a web page.

## Generic CSS Box Shadow Declaration

```bash
box-shadow: `offset-x | offset-y | blur-radius | spread-radius | color | inset;
```

1. `x-offset:` This represents the horizontal shadow position. A positive value puts the shadow on the right side of the box, a negative value puts the shadow on the left side of the box.
   If you want to apply a shadow equally to both the left and right sides of an element, you can do so by setting the horizontal offset (h-offset) to 0 and adjusting the blur and spread values.

2. `y-offset:` This represents the vertical shadow position. A positive value puts the shadow below the box, a negative value puts the shadow above the box1

3. `blur-radius:` **This is optional**. the higher the number, the more blurred the shadow will be and vice versa.

4. spread-radius: **This is optional**. A positive value increases the size of the shadow, a negative value decreases the size of the shadow1.

5. `color:` **This is optional**. The color of the shadow. The default value is the text color1.

**NOTE:** When styling the box-shadow property, remember that transparent shadows are the best because they look good on multicolored backgrounds. So always go in for `rgba` color model. The `rgba` color model allows you to specify the opacity of the color, which can create a transparent effect.

In `rgba`, the `a` stands for `alpha` and represents the opacity level of the color. The value of a can range from 0 (completely transparent) to 1 (completely opaque).

For example, `rgba(0, 0, 0, 0.5)` would represent a semi-transparent black color. When used in the box-shadow property, this would create a shadow that is partially transparent.This means the shadow will blend with whatever color is behind the element.

Transparent shadows can be beneficial because they blend well with different background colors. Instead of having a solid shadow that may clash with the background, a transparent shadow will take on some of the background color, leading to a more cohesive design.

6. `inset:` **This is optional**. This is optional.The insert property the shadow from an outer shadow (default) to an inner shadow. This means the shadow is drawn inside the element’s border, rather than outside of it.

The inset keyword is used at the beginning of the box-shadow property definition to specify that the shadow should be an inner shadow. If you place it at the end of the property definition, it will not be recognized correctly by the browser.

This is because the box-shadow property expects a specific order of values: `offset-x | offset-y | blur-radius | spread-radius | color | inset?.` The inset keyword is optional and comes last in this sequence. However, if it is included, it should come before the other values.

```bash
 .example1 {
  box-shadow: inset 5px 5px 10px rgba(0, 0, 0, 0.5);
}

```
