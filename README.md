# ZapTest
Skeleton for todo manager in android

## Overview
You will create a ToDo Manager application. The application creates and manages a list of ToDo Items (i.e., things that you need “to do.”). 

The main Activity for this application is called Lab4_UILabs. When the Activity runs, but there are no previously saved ToDo Items, its initial UI will have only a button: "Add New ToDo Item". This user interface contains a single ListView that displays all existing ToDo Items. As stated before, the last row of the ListView always displays a special View, with the words, “Add New ToDo Item.”.

When the user clicks on the ListView footer, the application will start a new Activity called AddToDo-Activity that allows the user to create and save a new ToDo Item.

ToDo items have at least the following fields. Default values appear in bold:
* Title: A user-provided String. The default Title is the empty String ("").
* Status: one of {Done, Not Done}
* Priority: one of {Low, Med, High}
* Time & Date: A deadline for completing this ToDo Item. The default deadline is 7 days from the current date and time.

This Activity's user interface includes the following buttons:
* Cancel – finish the Activity without creating a new ToDo Item.
* Reset – reset the fields of the ToDo Item to their default values and update the display to reflect this.
* Submit – create a new ToDo Item containing the user-entered / default data fields and return it to ToDoManagerActivity. When the application returns to ToDoManagerActivity, the new ToDo Item should appear in the ListView.

For example, if the user creates and submits a new ToDo Item to an empty ToDo list, then once the application returns to the ToDoManagerActivity, its ListView will contain the new ToDo Item.

Back in the Main Activity, the user will be able to toggle the Done checkbox to indicate that the ToDo Item's status has changed, say from Not Done to Done.


## What you have to do
1. First of all, fork this repository into your own GutHub profile;
2. After that, clone the code into your computer;
3. Then you need to look for every TODO in project and implement the code;
4. Run all tests and fix every bug until all tests are passing;
5. To finish, send to your interviewer the url to the GitHub repository.

### What you may do (only if you want to cause a good impression)
1. Right now the ToDo manager is quite ugly. Try modifying the layout files to create more attractive and useable layouts. For example, play with the font size of the text, the amount of padding around the elements, background colors and more;
2. Modify your application so that ToDoItems whose status is Not Done are displayed in the Main Activity with a different colored background than those whose status are Done. If you do this, then when the user toggles the Done checkbox, the background color should also change as appropriate. You might also consider changing the background color or adding a warning icon as the ToDo Item’s deadline get close. Finally, right now, the user can't modify the ToDoItem's priority from the ToDoItem ListView. Modify this user interface so that it provides a drop down list, allowing users to select a different Priority;
3. Modify your application so that if the user long presses a ToDo Item in the Main Activity’s ListView, a dialog pops up, allowing the user to delete the selected ToDo Item;
4. Implement this code with two Fragments and only one activity;
5. Create a specific layout for tablets.

## Tips
1. Do NOT modify any resource IDs contained in the skeleton layout files as this may break the test cases;
2. This project was created in Eclipse, but you can import it in Android Studio and it will work;
3. All tests must pass, but, beware, some tests will only work in API 17. I recommend you create a virtual device with this API level.
