# BMR-Diet-Program
A menu-based program to allow the dietician to input clients and their information. The menu should allow the dietician to:
- Enter client first and last name, body type, weight, height, age, and level of activity as described in the problem background
- Select a client
- determine daily calorie, fat calories, and fat grams needed
- choose a menu for breakfast, lunch, and dinner from a list of foods as in the problem background (you may add more to the list if desired) giving total daily food and fat calories
- recommend a reduced calorie intake if the client wishes to lose weight of 10% less calories than the daily calorie need; the reduced fat calories and grams should be given as well
- exit the program
### Case 1
User enters existing name.
<br />Result- Existing details displayed.
<br />User is asked the new details.
<br />Result-Existing details updated and daily calories need and required displayed.

### Case 2
User enters new name.
<br />User is asked the details.
<br />If user enters wrong type of values, he is prompted again.
<br />Result- New details added to the file with name and daily cal and other things displayed.

# Method/Algorithm

- Importing necessary libraries
- Taking input of client name
- Opening file for reading
- Opening file for writing(append)
- Checking if the name already exists and break search when found
- If exist, then print the previous details
- Taking input of all details of client and asking again until user enter right type of value
- If the name does not exist then append the details with name to the file
- Opening temporary file and writing in it and then moving its contents to original file at the end
- Checking if the name exists in the file. If yes then replace the details of name with new details in the temporary file
- Moving the contents of temporary file to original file
- Calculating bmr and hbf according to values entered by the user
- Asking user if he wishes to loose weight. If yes then show him new daily cal need
- Recommending food
