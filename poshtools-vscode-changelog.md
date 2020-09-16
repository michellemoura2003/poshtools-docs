---
description: Changelog for PowerShell Pro Tools for Visual Studio Code
---

# PowerShell Pro Tools for Visual Studio Code

### 5.13.1 - 9-13-2020

**Changed**

* Default install of trial license

### 5.13.0 - 9-1-2020

**Added**

* Added "Generate Tool" command

### 5.12.11 – 9-1-2020

**Changed**

* Updated to the latest version of PSScriptPad
* Fixed an issue with Form Generation where it would generate forms with common parameters

### 5.12.10 – 7-21-2020

**Added**

* PowerShell Pro Tools: Install PowerShell Pro Tools Module command

**Changed**

* Fixed an issue that would cause the extension to delay on startup and occasionally time out

### 5.12.9 – 7-16-2020

**Changed**

* Fixed an issue with PSScriptPad where the variables window wouldn’t expand variables correctly

### 5.12.8 – 7-15-2020

**Changed**

* Fixed an issue that would cause a delay on start up

### 5.12.5 – 7-12-2020

**Changed**

* Fixed an issue where ListView, TreeView and ContextMenu child items would not work in PSScriptPad
* VS Code extension now installs the PowerShell module automatically so it loads correctly
* Fixed an issue where packaging would fail if a script ended in a comment
* Fixed an issue where packaging would fail if a script was too large
* Fixed an issue where the opacity setting wouldn’t work on form controls on certain systems.

### 5.12.5 – 7-01-2020

**Changed**

* Fixed an issue where the PowerShell Pro Tools host process could lock up
* Fixed an issue where installing a license would report failure when it was actually succeeding.

### 5.12.4 – 6-26-2020

**Changed**

* Changed the license notification text and link as new licenses have been deployed to all affected customer’s accounts
* Fixed an issue where launching more than one version of VS Code would cause the extension to fail to connect

### 5.12.3 – 6-24-2020

**Changed**

* Fixed an issue where the extension could fail to connect to the PowerShell process.

### 5.12.2 – 6-23-2020

**Changed**

* The provider tree view now runs within the main runspace.

### 5.12.1 – 6-19-2020

**Added** 

* Added Host Processes tree node with support for one-click debugging runspaces

### 5.12.0 – 6-19-2020

**Added** 

* Added an Output Channel for PowerShell Pro Tools diagnostics

**Changed**

* PowerShell Pro Tools now uses an external process rather than being hosted directly in PowerShell
* Fixed an issue where the PowerShell Pro Tools module would load over and over again
* Fixed an issue where the variable window would not show variables
* Fixed an issue with the form designer that wouldn’t be marked dirty when properties were edited
* Fixed an issue with the form designer where it wouldn’t save StatusStrip items
* Fixed an issue with the form designer where it wouldn’t change the main PS1’s form name if it was changed in the designer
* Fixed an issue with the profiler where it would not work if params or using statements were used.

### 5.11.0 – 5-29-2020

**Added**

* Added support for packaging PowerShell 7 executables
* Added experimental support for packaging Linux and OSX executables

### 5.10.1 – 5-6-2020

**Changed**

* Fixed an issue with PSScriptPad that was causing hangs when running WinForm scripts.

### 5.10.0 – 4-17-2020

**Added**

* Out-VSCodeGridView

### 5.9.0 – 4-16-2020

**Added** 

* Cmdlets for managing [VS Code with PowerShell](https://ironmansoftware.com/automating-visual-studio-code-with-powershell/)

### 5.8.8 – 4-14-2020

**Changed**

* Fixed an issue with the variables view showing incorrect child items
* Improved the expansion of child items in the variables view
* Improved the generation of child item paths

### 5.8.7 – 4-6-2020

**Changed**

* Fixed an issue where putting an apostrophe in a label would cause the Form Designer to fail to load
* Fixed an issue where copy and pasting text into PSScriptPad would cause it to crash

### 5.8.6 – 4-3-2020

**Changed**

* Fixed an issue with the variable view not showing variables.

### 5.8.5 – 3-27-2020

**Added**

– Added a $Service object to OnStart\OnStop for packaged services to access the ServiceBase for the service  
– Added $ProcessArgs and $ServiceArgs variables to the runspace for packaged services

**Changed**

– Fixed an issue where $PSScriptRoot would not work for packaged services

### 5.8.4 – 3-3-2020

#### Changed

– Fixed an issue where an error would be shown when loading the extension– Fixed an error where loading the module tree would cause the extension to become unresponsive

### 5.8.3 – 2-10-2020

#### Changed

– Fixed an issue where a failed packaging build would not show the error message in the output

### 5.8.2 – 1-31-2020

#### Added

– Added -ProductId to New-Installer  
– Added -ScriptArguments to New-InstallerCustomAction  
– Added an option to add a context menu item for opening PS1 files with PSScriptPad  
– Added support for Comment \(Ctrl+K,Ctrl+C\) and Uncomment \(Ctrl+K,Ctrl+U\) keyboard shortcuts in PSScriptPad  
– Added support for reloading files updated outside of PSScriptPad

#### Changed

– Fixed issue with installer shortcuts throwing an exception if a workingDirectory or arguments were not specified  
– Fixed an issue where the installer shortcut working directory would not be specified correctly  
– Fixed an issue where the installer shortcut would not use the correct PowerShell variable  
– Fixed an issue where adding images to the installer UI on Windows PowerShell would throw an exception  
– Fixed an issue where PSScriptPad would crash on startup.

### 5.8.1 – 1-28-2020

#### Added

– Added support for WorkingDirectory on New-InstallerShortcut  
– Added support for Arguments on New-InstallerShortcut  
– Added support for Show on New-InstallerShortcut  
– Added support for Arguments on New-InstallerCustomAction

#### Changed

– Fixed issue where packaged applications wouldn’t work with arguments with spaces  
– Fixed issue with installer cmdlets not resolving paths correctly  
– When specifying a shortcut for an installer, if it’s a PS1, it will automatically launch PowerShell.exe rather than targeting the script

### \[5.8.0\] – \(1-22-2020\)

#### Changed

* No longer requires a [trial key](https://ironmansoftware.com/simplifying-product-trial-licensing/)

### \[5.7.1\] – \(1-21-2020\)

#### Changed

* PowerShellProTools module is now signed
* Fixed an issue with [PSScriptPad](https://ironmansoftware.com/psscriptpad/) that was preventing typing while IntelliSense was running in the terminal

### \[5.7.0\] – \(1-18-2020\)

#### Added

* Support for generating resources such as images and icons for WinForms.

#### Changed

* Fixed issue with packaging resources used for WinForms.

### \[5.6.6\] \(1-15-2020\)

#### Changed

* Fixed an issue where licensing would attempt to activate more than once and sometimes failing which resulted in some users not being able to use the tools.

### \[5.6.5\] \(1-14-2020\)

#### Changed

* Fixed an issue where packaging config would not respect the platform property.

### \[5.6.4\] \(1-13-2020\)

#### Changed

* Fixed an issue where packaging would use a package.psd1 in the temp directory.

### \[5.6.3\] \(1-12-2020\)

#### Changed

* Fixed an issue where packaging would throw an invalid format exception
* Fixed an issue with package architecture

### \[5.6.2\] \(1-10-2020\)

#### Added

* Added support for setting the architecture of the exectuable that is created when packaging

#### Changed

* Replaced Windows Form Designer with [PSScriptPad](https://ironmansoftware.com/psscriptpad/)
* Fixed an issue with ToolStrip items.
* Fixed an issue with deleting components

### \[5.6.1\] \(12-31-2019\)

#### Added

* Added breakpoint support to the Windows Form Designer
* Added stepping support to the Windows Form Designer
* Added support for stopping debugger to the Windows Form Designer

#### Changed

* Improved performance of IntelliSense
* Fixed a bug where the Windows Form Designer would lose code-behind changes on startup.

### \[5.6.0\] \(12-28-2019\)

#### Added

* The Windows Forms Designer can now execute PowerShell to show the form you are designing.
* The Windows Forms Designer can now package the Windows Form as a executable
* An output window was added to the Windows Forms Designer so you can see the output from your PS scripts.

### \[5.5.1\] \(12-20-2019\)

#### Changed

* Fixed an issue where the Actipro license was not installed correctly resulting in a popup.

### \[5.5.0\] \(12-20-2019\)

#### Added

* The Windows Forms Designer properties and toolbox are now in a dockable tool window.
* The Windows Forms Designer now supports moving controls with the arrow keys.

### \[5.4.6\] \(12-18-2019\)

### Added a button to open the Windows Form Designer

We’ve made it easier to open the Windows Form Designer from a PowerShell file. Just click the new Show Windows Form Designer button from your form.ps1 file.

[![](https://i2.wp.com/ironmansoftware.com/wp-content/uploads/2019/12/show-winform.png?resize=570%2C351&ssl=1)](https://i2.wp.com/ironmansoftware.com/wp-content/uploads/2019/12/show-winform.png?ssl=1)

### Fixed error message when executing commands

In certain circumstances, when you would execute PowerShell Pro Tools commands, an E\_PIPE error would be shown even though the command was completed successfully.
