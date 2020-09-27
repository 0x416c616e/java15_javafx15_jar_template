# Java 15 JavaFX 15 JAR Template

An easy way to make and launch a JavaFX 15 JAR. 

This requires JavaFX 15 (OpenJFX), Java 15, and IntelliJ.

This template makes it easy to make a JavaFX program that you can launch by just double clicking on something.

These instructions are intended for Windows. Maybe I will add macOS and Linux support in the future, but not now. macOS/Linux can do this mostly the same, but with different relative paths, and using a shell script instead of a .bat + a .vbs.

## Instructions

### Setup:

1. Clone the repo
2. Open the project folder in IntelliJ
3. Click File -> Project Structure -> Libraries -> Click the + icon -> Java
4. Navigate to the java15_javafx15_jar_template\openjfx-15_windows-x64_bin-sdk\\**lib** folder and select it
5. Click OK
6. Click OK when it says "Choose Modules"
7. Click Apply
8. Click OK
9. Click "Add Configuration"
11.  Click the + icon
12. Click Application
13. Type "Main" in the "Main class" field (without quotes)
15. Copy "--module-path openjfx-15_windows-x64_bin-sdk\javafx-sdk-15\lib --add-modules javafx.controls,javafx.fxml" to your clipboard (without quotes)
14. Click in the text field for the "VM options" section
15. hit ctrl+v
15. Click apply
16. Click OK
17. If you set up the configuration correctly, it should say "Main" and NOT "Unnamed"
18. If it says "Unnamed" then try just replacing either the "Main" or the VM options text again and hit apply and OK again, making sure that it still has the same values as before, but this time changing the name of the configuration to Main
18. Hit run to make sure you did everything correctly

### Coding in the template and then running the JAR:

1. In the left-hand tab, navigate to the Main file in the src folder
2. Write your code in the Main class
3. Run to make sure it works
4. Build -> Build Artifacts -> Build
5. Double click the run.vbs script
6. You are now running the JAR

### How to change the name of the JAR

Here's an example of how to change the name of the JAR. When you change the name of the JAR, there are a few other things that need to change.

1. Click File -> Project Structure -> Artifacts
2. In the "Name" field towards the top middle, rename "java15_jar_test:jar" to something like "my_program:jar" without quotes (if you use a different name, replace the following instructions' use of "my_program" to your own filename)
3. Under the part that says "Output Layout" look for the part that says "java15_jar_test.jar"
4. Right click "java15_jar_test.jar and hit "Rename"
5. Change the text to "my_program.jar" (without quotes) and hit enter
3. Click apply
4. Click OK
5. Click Build -> Build Artifacts -> my_program:jar -> Build
6. In an Explorer window, navigate to the java15_javafx15_jar_template folder
7. Right click on run.bat and hit edit to open it with notepad
8. On line 4, replace "cd java15_jar_test_jar" with "cd my_program_jar" (without quotes)
9. At the end of line 5, replace "java15_jar_test.jar" with "my_program.jar"
10. Save the file


