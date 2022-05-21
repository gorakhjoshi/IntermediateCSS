# Align-self

The `align-items` rule determines how all Flex-items inside a Flex container are aligned on the cross-axis.

Sometimes there are exceptions to this rule. For instance, suppose there are blog post thumbnails centered on the cross-axis. However, as we put the mouse cursor over a Flex item, we would like to stretch that one blog post thumbnail.

We can define similar exceptions on any Flex item using `align-self`.

> The cross-axis alignment of a Flex item is determined as follows:
>
> If there is an `align-self` rule defined on an individual Flex item, then this rule takes priority. Otherwise, the `align-items` property of the container determines the cross-axis alignment of the Flex item.

There is one more caveat that determines if `align-self` has an effect on the cross-axis alignment of a Flex item: the Flex container has to have a defined cross-axis dimension.

- For `row` or `row-reverse` Flexboxes, `height` has to be defined on the container.
- For `column` or `column-reverse` Flexboxes, `width` has to be defined on the container.

## align-self with horizontal flex-direction

Let’s examine the possible values for `align-self` in the case of horizontal `flex-direction`:
![Align-self with flex-direction row](images/Align-self%20with%20flex-direction%20row.png)

Please click the link below:

[Click here](https://codesandbox.io/s/angry-bird-0o8x0f)

## Align-self with vertical flex-direction

When `flex-direction` is vertical (`column` or `column-reverse`), align-self performs horizontal alignment:

![output](images/Align-self%20with%20flex-direction%20column.png)

Please click the link below:

[Click here](https://codesandbox.io/s/infallible-tharp-tekd5u)
