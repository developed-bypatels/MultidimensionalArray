Background
Developed a program that will analyze a set of elevation data collected in a text file. The text file is formatted as a series of rows and columns. The first row will contain two values that are the number of rows of data followed by the number of columns. All of the values in the data file are integer values in the range of 0 to 9500 inclusive. This is an absolute range and it is known that the data will reside within this range. However, the range of data could be smaller than the absolute range. See the Lab#1 dropbox folder for a copy of the data file called ELEVATIONS.TXT.
Requirements
You must determine the following about the data set:
• Print the lowest elevation value and the number of times it is found in the complete
data set. Also print the row and col of the value closest to the top left corner of the data set. See example below:
012345
0 21 33 44 12 59 32
1 12 11 10 18 19 21
2 10 44 99 12 13 10
3 96 44 55 12 10 67
4 23 33 12 33 10 65
     5     32 12 77 99 73 43
You will notice that 10 is the lowest value in the data set and it occurs 5 times. The location closest to the top corner if we start counting at row 0 column 0 will be the value at row 2 column 0 since the distance is closer than the distance of the 10 value found at row 1 column 2. Use Pythagoras theorem for calculating distance.
𝑑𝑑2 = 𝑟𝑟2 + 𝑐𝑐2
where d is the distance
r is the row number (consider the first row as row 0)
c is the column number (consider the first column as column 0)
• Print the total number of local peaks that occur in the data set where the peak elevation is in the range from 8900 to 9000 inclusive. A local peak occurs when a value is higher
than all of the values within 2 rows and columns inclusive in all directions of the data set. local peaks in the first two rows, first two columns, last two rows and last two columns can be excluded from the analysis. See example below on a 10 x 10 data set where we are interested in all local peaks between 90 and 99 inclusive:
0123456789
0 21 33 44 12 59 32 77 66 44 11
1 12 11 10 18 19 21 61 23 95 14
2 10 44 99 12 13 10 55 44 41 65
3 96 44 55 12 10 67 23 32 65 43
4 23 33 12 33 10 65 87 66 53 41
5 32 12 77 98 73 43 33 12 42 23
6 37 62 27 43 61 11 12 91 33 12
7 76 19 43 57 64 77 81 73 43 29
8 18 21 37 98 19 71 44 83 11 42
9 12 42 77 75 73 88 13 22 52 28
There are 3 local peaks which occur are 99(2,2), 98(5,3) and 91(7,6). Note that although
95 and 98 are examples of local peaks they occur in the excluded area.
• Print the row and column of the two closest local peaks using the formula for distance
presented earlier. In the data presented above the min distance would be 3.16 (the two peaks located at (2,2 with an elevation of 99) and (5,3 with an elevation of 98). Print the distance to 2 decimal places.
• Print the most common elevation in the data set. In the data set presented above the most common value is 12 and it occurs 11 times.
