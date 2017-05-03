### Setup
* From address book directory, run yarn install, yarn start

### Do
* Import the array of users into index.js
* Create a folder in src called components to hold all our components
* Create the UserDetail and ListOfUsers functional components
* Import and use components in App
* Send the user array into Apps and then into ListOfUsers
* Send the first user from the array down into the UserDetail component

### Favorites list
* Create another list of users with the headline "Selected users" next to the other list
* Initially, this list should show "No users selected"
* Add a button to the existing list of users with the label "Select user"
* When you click on that button, the user should be removed from the original user list and should be moved to the "Selected users" list
* In the "Selected users" list you should then see the users with a button "Deselect user"
* On click on "Deselect user" the user should be moved back
* Add a button that resets the whole application to its initial state (no page reload allowed)

### Action History
We are going to implement an action history that records the user's actions. Implement the following functionality:

- Add a new container with a headline "Action history" underneath or right next to your two lists.
- The initial message should show something like this: "You have not performed any actions yet."
- The following messages should appear in the action history and should be added to the top of the list (Examples):
  - You have selected "Dale Cooper, FBI Agent"
  - You removed "Dale Cooper, FBI Agent" from your selection
  - All contacts were removed
  - The application was reset to its initial state
- Add a button to the bottom of the list, that clears the action history.
- The maximum number of action items should be limited to 10 entries. Only the most recent entries should be displayed. (If you have more than 10 items in your action history and you delete an entry, you should only see 9 entries)
- Implement an expiration time for the action history that automatically removes all entires that are older than 1 minute. You will have to use component lifecycle methods for that. Read up on it in the react documentation.
- Add a button (X) to each action item that lets the user remove an item from the action history.
