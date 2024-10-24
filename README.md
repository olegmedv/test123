# Exercise - Flexbox

## Step 1: Experiment with min-width

The flex container has a width of 50%. The items have a flex-basis of 200px.
In the .item rule, the min-width is set to 100px. This prevents the Flex items from shrinking below 100px, no matter how small the screen gets.

1. Resize the browser to see how the items behave when the screen width is reduced. The items won’t shrink below 100px.
2. With the window small, open the browser developer tools and inspect the item, see how the interface shows that the item was shrunk.
3. Try playing with the min-width value and see how the layout changes.

## Step 2: Use flex-basis

1. The flex-basis property in the .item class is set to 200px. This sets the starting size of each Flex item.
2. Modify flex-basis to different values (e.g., 50px, 100px, 300px) and observe how the items adjust.
3. Notice that flex-basis defines the default size of items before any growing or shrinking happens.

## Step 5: Adjust flex-grow

1. Add flex-grow: 1; to the .item class. This tells Flex items to grow and take up available space equally.
2. Make the browser window wide, now, the Flex items will expand to fill any remaining space in the container.
3. To see the effect better, try setting flex-grow to different values for each item (e.g., flex-grow: 1; for the first item and flex-grow: 2; for the second). The default value is 0. Items with a higher flex-grow value will expand more.

## Step 6: Control with flex-shrink

By default, all items shrink equally when necessary, but you can control how much they shrink by adjusting the flex-shrink value. The default value is 1.

1. Try setting flex-shrink: 0; for one item.
2. Make the browser window smaller to see the effect. The item with flex-shrink: 0; won’t shrink, while others will.

## Step 7: Add gap for Spacing

The gap property is already applied to your Flex container with gap: 10px;, which creates 10px space between each Flex item.

1. Change the gap value (e.g., 20px, 50px) to see how the spacing between items changes. The gap property is a cleaner alternative to adding margins between Flex items.

## Step 8: Use auto Margins for Alignment

1. Remove flex-grow and flex-shrink from the .items rule and refresh your browser window.
2. To experiment with auto margins, add margin: auto; to the second item. The CSS selector below uses a pseudo class:

```
.item:nth-child(2) {
margin-left: auto;
}
```

3. Resize your browser window to see the effect. This will push the second item to the far right of the container.

4. Try applying margin: auto; to different items and see how it changes their alignment within the container.

## Step 9: Challenge - Combine Everything

Now that you understand each property, create a layout that uses min-width, flex-basis, flex-grow, flex-shrink, gap, and auto margins in creative ways.

1. Remove flex-basis and min-width from the .items rule and refresh your browser window.
2. Make the first item stay at a fixed size using flex-basis and min-width.
3. Let the second item grow and shrink based on the container size using flex-grow and flex-shrink.
4. Use auto margins to align the third item to the right. Can you do that? Why not? What would you have to change to make the auto margin take effect?
