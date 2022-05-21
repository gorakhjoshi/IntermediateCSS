# Flex Shrink

While `flex-grow` distributes the available space in a Flexbox container to grow flex-items, `flex-shrink` takes away from the basis of Flex components when there is not enough space for them.

Similar to `flex-grow`, items can also shrink proportionally with respect to the ratio of their `flex-shrink` values. The higher the flex-shrink value, the more an element will give up from itself with respect to other items to fit in its Flexbox container.

Shrinking is performed proportionally based on the individual `flex-shrink` and `flex-basis` values.

![flex-shrink](images/flex-basis%2C%20flex-shrink.png)

Please click the link below:

[Click here](https://codesandbox.io/s/flex-shrink-erm7df?file=/src/styles.css)

The fourth example may require some explanation. We shrink the elements from `900px` to `600px`. Shrinking is performed in the proportion of the `flex-shrink` values of the individual items. The first item shrinks `60px`, the second shrinks four times as much: `240px`.
