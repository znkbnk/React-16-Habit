1. Category Dropdown.

- Create a new file named CategoryDropdown.js in
the same directory as your other components.
- In CategoryDropdown.js, define a functional
component for the category dropdown.
- Inside the component, render the list of categories
(e.g., "All", "Read", "Drink Water", "Do Exercise")
using the map function.
- Implement a function that handles category selection.
- This function should call a callback function
passed as a prop (e.g., onCategorySelect).
- Add logic to show/hide the dropdown when a button 
(e.g., "Categories") is clicked. You can use state
(e.g., useState) to manage the visibility.
- Apply CSS styles to the dropdown to make it
visually appealing. You can use class names 
and CSS stylesheets for this.
- In your App.js, import the CategoryDropdown component.
- Include the CategoryDropdown component in your 
app's render, passing the necessary props
(e.g., showCategoriesDropdown, onCategorySelect).

2. Selected Category.
   
- In your App.js, use useState to initialize state 
variables for selectedCategory and showCategoriesDropdown.
- Update the props you pass to the HabitForm and
HabitList components to include selectedCategory.
- Implement a function (e.g., handleCategorySelect)
to update the selectedCategory state when a category
is selected in the dropdown. Pass this function
as a prop to the CategoryDropdown component.

3. Category Property in Habit.

- In your HabitForm.js, modify the habit object to include
a category property. Update the form input fields and
state accordingly to capture the selected category.
- Ensure that a category is selected before allowing the
user to add a habit. You can display an error message
if no category is selected.
- In HabitList.js, update the rendering logic to display
the category for each habit (e.g., {habit.category}).

4. Goal Days Validation.

- In your HabitForm.js, implement validation for the
"goal days" input field to ensure it's a positive number.
- You can use JavaScript conditions (e.g., if) to check
the input value.
- If the goal days are invalid (not a positive number),
display an error message (e.g., <p style={{ color: "red" }}>
Number must be higher than 0</p>) to guide the user.
- Clear the error message when the user enters a valid goal
days value. You can do this by updating the error state
when the input is valid.
