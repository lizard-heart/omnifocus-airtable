# omnifocus-airtable
OmniFocus plugin to sync from an air table database to omnifocus.


## setup
- Go to https://console.firebase.google.com 
- Login if you need to and create a new project 
- Enter any name, agree to terms, (you don't need google analytics) 
- Go to Build -> Firestore Database -> create database -> next -> enable 
- Start a collection with any id (use the id "projects" if you want it to match with the code I wrote) and in the initial document put a field called name (a string) and if you want a field called is_completed or something (boolean) 
- Lastly, go over to the rules and change false to true. 
- Finally, firebase is all setup. Now create a zapier to send data from Airtable to firebase. Use this link as a template: https://zapier.com/shared/8b72c5940a3edb3e0621a817319d63dda3cc5e93 
- Lastly, install the attached plugin. Before you install it, you'll have to edit the first line to make it match your firebase database. 
- Now, running that plugin should automatically complete all the projects that need to be completed in OmniFocus. 
