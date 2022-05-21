# Flex-grow and flex-basis

One reason why Flexbox is flexible is that Flexbox items can grow and shrink in size.

By default, each Flex item is displayed based on their `min-width` property.

Once one Flex item receives a positive `flex-grow` value, this item takes all the available space in the container.

If all the Flex-items receive the same positive `flex-grow` value, they divide all the available space among them equally.

We can adjust the proportions with respect to each other by assigning different positive flex-grow values to each Flex item. For instance, if the first item has a `flex-grow` value of 1 and the second item has a flex-grow value of 3, the second item grows three times as fast as the first value.

Example:

![flex-grow](images/flex-grow%20examples.png)

Please click the link below:

[Click here](https://codesandbox.io/s/flex-grow-7u301k)

In the last two Flexboxes, the black ruler at the bottom reads: “Exact widths cannot be revealed without setting flex-basis.”. Therefore, to calculate the exact widths, we will have to base the width calculation on `flex-basis`.

For instance, if `flex-basis` was set to `150px` for each element, the size of the container was `600px`, and there are two containers in total, then the remaining space would be allocated to the two items in the proportion of their `flex-grow` values. If the first element has a `flex-grow` of 1 and the second element has a `flex-grow` of 3, then:

- The first component receives 1/4th of the available `300px` horizontal space on top of its `150px` basis, yielding `225px`.
- The second component receives 3/4th of the available `300px` space on top of its `150px` basis yielding `375px`.

![flex-grow with flex-bsisx](images/flex-grow%20with%20flex-basis.png)

Please click the link below:

[Click here](https://codesandbox.io/s/flex-grow-with-flex-basis-lc7msm)
