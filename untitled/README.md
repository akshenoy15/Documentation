# Create a JSON file

Let us create a JSON file with structured data that captures the activities of the librarian and library patron.

**Step 1: Create a  library object.**

First, we need to create the main object named _library,_ which will be the outermost object. Objects are enclosed within curly brackets.

```javascript
{
   "library": []
}
```

Here we have a key “_library_”, but no value after the colon. Instead of value, we have a set of square brackets. Square brackets represent an array of data. Right now, the array is empty, meaning it is a list of zero items.

**Step 2: Create column objects within the library object.**

```javascript
{
   "library": [
      {
         "librarian": {}
      },
      {
         "library patron": {}
      }
   ]
}
```

In this example, we see that _librarian_ and _library patron_ are the entries, which are separated by a **,\(comma\)** in an array. The item _librarian_ and _library patron_ are two different objects which have their own set of entries.

**Step 3: Create item objects within the column objects of the library system.**

* Add entries to the _librarian_ object within curly brackets which are currently empty, representing zero items.

```javascript
{
   "library":[
      {
         "librarian":{
            "check_out":{
               "book_title":"our planet",
               "check_out date":"01-01-2021"
            },
            "check_in":{
               "book_title":" ",
               "check_in date":" "
            },
            "pay_fine":" ",
            "add_book":" ",
            "report_stolen":" ",
            "new_membership":" ",
            "cancel_membership":" "
         }
      }
   ]
}
```

* Add entries to _library patron_ object.

```javascript
{
   "library":[
      {
         "lib_patron":{
            "check_out":[
               {
                  "book_title":" ",
                  "check_out date":" "
               }
            ],
            "check_in":" ",
            "pay_fine":" "
         }
      }
   ]
}
```

The final file with all the object entries should look like [this](https://gist.githubusercontent.com/akshenoy15/5dee392df23d79fe1d30568ecc0233f7/raw/764b83857bc0acdc3da2325f690d59082c1e364d/library_admin_system.json).





