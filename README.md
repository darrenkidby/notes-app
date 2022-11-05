# notes-app

01. Adding a Menu
I needed to add, Add a note, List all notes, Update a note Delete a note and exit as options for the user to click.

    1. mainMenu() function
    I needed to add the variable val scanner = Scanner(System.`in`)
    as well as a few println() to create the menu.

    2. runMenu function
    I needed to add the functions so when the user typed the number that was beside the option, it chooses the users choice.

    3. remaining functions
    I added skeleton code for addNote(), listNotes(), updateNote(), deleteNote() and exitApp. This will be updated later.

02. Refactoring Menu Code

    1. I changed the println() menu to one singular print() with all options inside.

03. Input Mismatch Exception

    1. I created a new package called utils and in the package a file called ScannerInput and added the needed code into it.
    2. I added code in the mainMenu() to allow the contents of the print statement is sent as a parameter in the ScannerInput() function.

04. Adding Logging Support

    1. I added two new dependencies to build.gradle.kts
    2. In the main.kt I added private val logger = KotlinLogging.logger {} 
    and updated the addNote() skeleton code.

05. Issues

    1. I created an issue about adding notes.
    2. I created a second issue about JUnit automated testing.

06. Branches

    1. I created a branch to help solve issue one, I called the branch collection-and-model.
    2. I created a new package called models and added a kotlin class called Note in this package, I also added code to the Note file.
    3. I committed these new changes to the new branch.

07. Collection

    1. I created a new package called controllers and added a kotlin class called NoteAPI in this package, I added the relevant code to this file.
    2. I added a variable to the main.kt to allow this file to work.
    3. I added code to the addNote() function to make the add work.
    4. I also updated the listNotes() skeleton code.

08. Pull Request

    1. I clicked Compare & pull request on my GitHub page and created the pull request. 
    2. I added issue one to this pull request.
    3. I merged the pull request.
    4. I deleted the branch from the GitHub.
    5. I used git fetch on intellij to delete the remote collection-and-model branch.
    6. I clicked checkout on the Master remote branch.
    7. I manually deleted the local collection-and-model branch.

09. Testing

    1. I added test code to noteAPItest
    2. I ran the tests to see if they were working.
    3. I did the same as the 08. Pull Request section.

10. List and Number

    1. I added the code to work listActiveNotes(), listArchivedNotes(), numberOfArchivedNotes() and numberOfActiveNotes().
    2. I added the associated test code.
    3. I created the issue branch and used a pull request to close the issue.
    4. I added the code to work listNotesBySelectedPriority(priority: Int) and numberOfNotesByPriority(priority: Int).
    5. I added the associated test code.
    6. I created the issue branch and used a pull request to close the issue.

11. New Issues

    1. Created an issue for Update.
    2. Created an issue for Delete.
    3. Created an issue Persist for JSON or XML.

12. Update Note

    1. Created a branch for the update function.
    2. I added code in noteAPI to make the updateNote() work.
    3. I added code to the main.kt.
    4. I added the test code for the update.
    5. I committed and pushed the code. Created a pull request to close the issue and deleted the branch.

13. Update Note

    1. Created a branch for the delete function.
    2. I added code in noteAPI to make the deleteNote() work.
    3. I added code to the main.kt.
    4. I added the test code for the delete.
    5. I committed and pushed the code. Created a pull request to close the issue and deleted the branch.

14. Persistence XML and JSON

    1. Created a branch for the Persistence.
    2. I created a new package called persistence and added three new kotlin classes called Serializer, JSONSerializer and XMLSerializer.
    3. I added the relevant code to the Serializer file.
    4. I added new dependencies to build.gradle.kts.
    5. I added the relevant code to the XMLSerializer file.
    6. I added code for the XMLSerializer in NoteAPI and Main.kt
    7. I added to new menu items in save() and load()
    8. I added testing for XML in NoteAPItest.
    9. I committed and pushed the code.
    10. I added the relevant code to the JSONSerializer file.
    11. I added code for the JSONSerializer in NoteAPI and Main.kt
    12. I added testing for JSON in NoteAPItest.
    13. I committed and pushed the code. Created a pull request to close the issue and deleted the branch.

15. Archive Note

    1. I added code to noteAPI for archiveNote().
    2. I updated the menu changes for archive note.
    3. I added code to main.kt to make archiveNote() work as well as listActiveNotes().
    4. I created a test that was associated with this.
    5. I used a pull request and deleted the branch.

16. Submenu

    1. I added a submenu for listNotes and added new functions.

17. Tracked Files

    1. I added /build in .gitignore so it would ignore all the build folder.
    2. Using the terminal, I stopped the tracking for these files.
    3. I did the same for the .gradle files.

18. Lambdas Counting

    1. I added a new issue and branch.
    2. I added the relevant test code.
    3. I made the numberOfActiveNotes(), numberOfArchivedNotes() and numberOfNotesByPriority(priority: Int) easier to read.
    4. I committed and pushed as well as use a pull request and deleted the branch.

19. Lambdas List All

    1. I added a new issue and branch.
    2. I added the relevant test code.
    3. I made listAllNotes() easier to read.
    4. I committed and pushed as well as use a pull request and deleted the branch.

20. Lambdas Listing

    1. I added a new issue and branch.
    2. I added the relevant test code.
    3. I made listArchivedNotes() and listActiveNotes() easier to read.
    4. I committed and pushed as well as use a pull request and deleted the branch.

21. Lambdas Searching

    1. I added a new issue and branch.
    2. I created a new function called searchByTitle.
    3. In main.kt I added a new menu item for search.
    4. In noteAPITest, I added the relevant test.
    5. I committed and pushed as well as use a pull request and deleted the branch.

22. Lambdas Refactoring

    1. I added a new issue and branch.
    2. I refactored the joinString code.
    3. I checked the tests.
    4. I refactored the counting methods code.
    5. I checked the tests.
    6. I committed and pushed as well as use a pull request and deleted the branch.

23. Additional

    1. I added colour to the console. I found a GitHub webpage by mgumiero9 with different Ansi codes. https://gist.github.com/mgumiero9/665ab5f0e5e7e46cb049c1544a00e29f.