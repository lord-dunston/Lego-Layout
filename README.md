Lego Layout - Created by Ben Hall - 16/07/92

This Grid system allows you to build a site as simple as using Lego to build a model.

You will be able to see from the Lego-Layout.css file how the code works.

Each Column is place inside a "row" div which has a width of 100%. This means that the "row" div will always be 
100% of the width of the "wrapper" div.

Each column is 80px wide (before padding is added). This means to create a column that spans the width of 11 columns, 
we multiply 80 by 11. This gives us the width of 11 columns. We then divide that number by 960 and then multiply by 100 to
get the percentage width of the column.

To fill the remaining width of the "row" div we divide 80 by 960 and multiply by 100 to get the second column percentage width and add that 
column in to the "row" div.

You can add as much padding as you like as the top lines of code means that the width of the columns will always stay the same no matter how 
much padding is added.

The max-width of the wrapper is "960px". However this can be changed and the layout should not break. This is because the widths of the columns
add up to

The grid at the bottom divides the "row" in to twelfths. For example, you will be able to see that it is divided in to 1 row of 2 columns and 
1 row of 3 columns. This is reflected in the class name:

e.g.
col-1-3 is equal to 1 row - 3 columns.

This can be used in conjunction with the "Spans" above. For example, you may wish to have 4 columns in a span of 8 this can be done by simply:
1. creating a div with a class of "row".
2. adding in a div with a "col span-8 col-rp" class. The "col-rp" class will remove any padding added to the "span" so that the columns fill
   the width of the span.
3. add in 4 column divs with a class of "col-1-4".