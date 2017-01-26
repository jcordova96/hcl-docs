# Selenium IDE Installation and Usage

## Installation

### Install Firefox
- Install most recent version of Firefox.

### Install Selenium IDE
- Open Firefox, go to: https://addons.mozilla.org/en-US/firefox/
- In the "search for add-ons" search box, enter "Selenium".
- Install the following add-ons:

#### Required:
- Selenium IDE
- Highlight Elements (Selenium IDE)
- Stored Variables (Selenium IDE)

#### Recommended:
- Selenium IDE Button
- Favorites (Selenium IDE)
- Test Results (Selenium IDE)
- File Logging (Selenium IDE)
- Power Debugger (Selenium IDE)
- ScreenShot on Fail (Selenium IDE)
- SelBlocks (for Selenium IDE)

- You must restart Firefox for the add-ons to load.

## Install HCL Selenium Test Environment

If you would like to contribute to any HCL CnE Website Selenium IDE Test Suites or Test Cases, you will need to join our development environment hosted here: [https://hcl-cne.visualstudio.com/selenium-ide-tests/<nowiki>_</nowiki>home](https://hcl-cne.visualstudio.com/selenium-ide-tests/_home)

To do this please follow the steps below:

### Install Git and SourceTree (Git client)
- Go to: https://git-for-windows.github.io/
- Download and Install the installer with default settings.
- Go to: https://www.sourcetreeapp.com/
- Download and Install the installer.
- Open SourceTree.  No need to for Mercurial, No need for Github or Bitbucket account.
- Go to: File -> Clone/New.
- Under the "Clone Repository" tab, in the "Source Path / URL" field, paste [https://hcl-cne.visualstudio.com/<nowiki>_</nowiki>git/selenium-ide-tests](https://hcl-cne.visualstudio.com/_git/selenium-ide-tests)
- Click "Clone" button.
- When prompted for a username and password, enter your Microsoft credentials.

### Git Reference
- For more information on using Git (adding, committing, pushing, pulling, etc.), please consult the following references:
- https://git-scm.com/docs

## Usage
- Open Firefox.
- Open Selenium IDE by going to "Open menu" -> "Developer" -> "Selenium IDE".  Or you can use the shortcut Ctrl+Alt+S.

### Open an existing Test Suite
- If you have followed the steps in "Install HCL Selenium Test Environment", you can load or update any Test Suites/Cases created by our team.
- Each website in CnE has a different folder for each collection being tested (ex: Main), and for each of it's viewports being tested (desktop, table, mobile).
- In each folder there is exactly one Test Suite named with the naming convention {site}-test-suite-{collection}-{viewport}.
- Go to File -> Open Test Suite... then browse to the Test Suite file to open.

### Creating a new Test Suite
- If you are creating a new Test Suite for your HCL Cne environment, the best way to create it is to copy an existing folder and rename the files and folder appropriately.
- All of the data files saved by Selenium IDE are in HTML format.  Therefore they can be easily modified in Windows Explorer to rename and delete files/folders, and the files can be edited by your code editor of choice (Visual Studio Code, Sublime, etc.).
- Make sure that your folder contains the files: {site}-variables-{collection}.html, {site}-test-suite-{collection}-{viewport}.html with the proper values set.

### Adding Test Cases
- Our Test Case files correspond to a page, and should be named the page name.
- Right click on the "Test Case" pane and choose "Add Test Case..." or use the shortcut Ctrl+D.
- In the "Test Case" pane, the active Test Case is bolded.  Make sure your test case is active before trying to save it.  You can do this by double-clicking it.
- To save the Test Case go to: File -> Save Test Case.  Make sure to save your Test Case in the right folder.

### Record User Event Commands
- Once you have a Test Case open that you want to add commands to, you can begin by recording the user interactions you would like added to your Test Case.
- Make sure your Firefox browser window only has one tab and it is on the page you would like to test.
- On the Selenium IDE window, go to: Actions -> Record, or click the red "Click to Record" button.
- Now go back to your browser window and start performing your sequence of clicks, etc. that you want recorded for testing.
- When done, you can click the Record button again to stop recording.

### Playing Your Command List
- Click the "Play current test case" button.

### Add Testing Commands
- Now you have a set of commands recorded in the "Table" pane.
- Add more commands between the user event commands by right clicking on the "Table" pane and choosing "Insert New Command".
- Highlight your newly created command and choose the "Command" from the dropdown below and set the proper parameters in the "Target" and "Value" fields.
- Most commonly you will be adding commands to verify/assert data on the page.
- Try Test Suites/Cases already created by our team to see examples of how to structure your tests.
- Always add comments between groups of commands to make your Test Case readable.  Right-click on the "Table" pane -> Insert New Comment.

### Selenium IDE Documentation
- The Selenium IDE official website has very nice documentation and it's highly recommended to read through this to get a good understanding of using Selenium IDE to it's full potential:
http://www.seleniumhq.org/docs/02_selenium_ide.jsp






