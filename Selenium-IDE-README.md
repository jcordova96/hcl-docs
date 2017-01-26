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
- All of the data files saved by Selenium IDE are in HTML format.  Therefore they can be easily modified in Windows Explorer to change filenames and delete files, and the files can be edited by your code editor of choice (Visual Studio Code, Sublime, etc.).
- Make sure that your folder contains: {site}-variables-{collection}.html, {site}-test-suite-{collection}-{viewport}.html with the proper values set.






