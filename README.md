# LeadBoard  https://tejaskarde21.github.io/LeadBoard/day13LeadBord/index.html;

*The code starts by selecting various HTML elements by their IDs and assigning them to JavaScript variables:
input, fName, lName, country, score, Add, and output represent various form input fields and an output container,
likely corresponding to an HTML form for entering user information and an area to display the user data.

*An event listener is added to the "Add" button (Add.addEventListener). When this button is clicked, the following actions take place:
a. User input values (first name, last name, country, and score) are retrieved from the corresponding form fields.
b. A new div element with the ID "newOutput" is created using document.createElement.
c. Inside this new div, the user's information is added using template literals, creating a structured layout for each user's data.
d. The newly created div is appended as a child to the output container, effectively displaying the user's data in the web page.
e. The form input fields (first name, last name, country, and score) are cleared.
f. The sortBoard function is called to sort and re-order the displayed user data based on their scores.

The deleteButtons variable selects all elements with the class "delete" within the newly added user entries.
For each of these elements, an event listener is added to handle click events. When a delete button is clicked:
a. It identifies the parent element (the div with the ID "newOutput") that contains the user's data.
b. It removes this parent element from the DOM, effectively deleting the corresponding user entry.
