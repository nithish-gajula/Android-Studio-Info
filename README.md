# Android-Studio-Info

### Duplicating a project
```
cd /home/icps1101/Downloads/projects
cp -r "EasyMarkdown" "TestingMarkdown"
```

Step 2 – Open the Duplicate in Android Studio
In Android Studio:
**File → Open… → Select TestingMarkdown**
Wait for Gradle sync to complete.

Step 3 – Change the Application Name (UI label)
Open: app/src/main/res/values/strings.xml
Edit
```<string name="app_name">Easy Markdown</string>```
Change to:
```<string name="app_name">Testing Markdown</string>```


In the Project view (set to Android mode), expand:

```app/java/com/example/easymarkdown```
Right-click on ```easymarkdown → Refactor → Rename → type testingmarkdown.```

Android Studio will ask if you want to search in comments/strings — check it.

After renaming, open app/build.gradle and update applicationId to match the new package path:

applicationId "com.nithishgajula.testingmarkdown"
