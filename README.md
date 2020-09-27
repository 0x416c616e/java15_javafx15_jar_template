# Java 15 JavaFX 15 JAR Template

An easy way to make and launch a JavaFX 15 JAR

This requires JavaFX 15 (OpenJFX), Java 15, and IntelliJ.

This template makes it easy to make a JavaFX program that you can launch by just double clicking on something.

## Instructions

### Setup:

1. Clone the repo
2. Open the project folder in IntelliJ
3. Click File -> Project Structure -> Libraries -> Click the + icon -> Java
4. Navigate to the java15_javafx15_jar_template\openjfx-15_windows-x64_bin-sdk\*lib* folder and select it
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
18. Hit run to make sure you did everything correctly

### Coding in the template and then running the JAR:

7. Write your code in the Main class
8. Run to make sure it works
9. Build -> Build Artifacts -> Build
10. Double click the run.vbs script
11. You are now running the JAR

