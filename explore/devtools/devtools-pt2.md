1. The bug in explore.js was that num1 and num2 are strings and when added together, they create a concatenated string instead of producing the sum of their numerical values.
2. I fixed this bug by using parseInt() to cast num1 and num2 to integers and storing their sum in result.
