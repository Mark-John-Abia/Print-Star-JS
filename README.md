function printPyramid(rows) {
  for (let i = 1; i <= rows; i++) {
    // Print leading spaces
    let spaces = ' '.repeat(rows - i);

    // Print stars
    let stars = '*'.repeat(2 * i - 1);

    // Combine spaces and stars and print the row
    console.log(spaces + stars);
  }
}

// Call the function with desired number of rows
printPyramid(5);

/////////////////////////////////////////////////////////


Explanation:
Looping through the rows: We use a for loop to iterate over each row of the pyramid.
Spaces: For each row, we calculate how many spaces are needed to align the stars. The number of spaces decreases as the row number increases.
Stars: The number of stars on each row is calculated using the formula 2 * i - 1 (where i is the current row number). This ensures an odd number of stars.
Combining spaces and stars: For each row, we concatenate the spaces and stars and print them.

    *
   ***
  *****
 *******
*********


You can adjust the rows parameter in the printPyramid function to create larger or smaller pyramids!

The expression 2 * i - 1 is used to calculate the number of stars (*) that should be printed on each row of the pyramid. Here's the breakdown of why it's used:

i is the row number, starting from 1.
To form a symmetrical pyramid, the first row has 1 star, the second row has 3 stars, the third row has 5 stars, and so on.
The formula 2 * i - 1 helps generate this odd-numbered sequence of stars.

How it works:
For row 1 (i = 1):

2 * 1 - 1 = 1
The first row has 1 star (*).
For row 2 (i = 2):

2 * 2 - 1 = 3
The second row has 3 stars (***).
For row 3 (i = 3):

2 * 3 - 1 = 5
The third row has 5 stars (*****).
For row 4 (i = 4):

2 * 4 - 1 = 7
The fourth row has 7 stars (*******).
And so on.

So, 2 * i - 1 is essentially the formula to ensure that each row has the correct number of stars, following the pattern of 1, 3, 5, 7, etc., as you move down the rows of the pyramid.

Example:
For i = 5:

2 * 5 - 1 = 9
The fifth row will have 9 stars.
This ensures the pyramid shape expands correctly as the row number increases!# Print-Star-JS
