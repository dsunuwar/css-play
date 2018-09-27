There are two schools of thought when approaching gutters;

1. defining paddings within each column
2. using percentage based left margin for each column

The main advantage of first approach is, it makes column width calculation very easy.
For example,
width of 1 column = 100% / 12 = 8.33%
Now you determine width for each column totaling 100% for column 12.

The second approach is better for creating responsive gutters. But the column width calculation is a little bit more than just diving by 12. Assuming it's a 12 column grid, below is how we calculate widths,

Width of single column:
scw = (100 – (m x (mc – 1))) / mc

where,
scw = single column width
m = margin (1.6%)
mc = maximum columns (12)

scw = (100 - (1.6 x (12 - 1))) / 12 = 6.86666666667

When we plug in the numbers, we get a single column width of 6.86666666667%. From here we can use this number to calculate the rest of the column widths. The formula for this is:

cw = (scw x cs) + (m x (cs – 1))

Where:

cw = column width
scw = single column width (6.86666666667%)
cs = column span (1-12)
m = margin (1.6%)
