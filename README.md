# javascript
Basics of Javascript
# run in browser
For Windows - Open your Default Browser - Tested on VS Code v 1.1.0

Answer to both opening a specific file (name is hard-coded) OR opening ANY other file.

Steps:

Use ctrl + shift + p (or F1) to open the Command Palette.

Type in Tasks: Configure Task or on older versions Configure Task Runner. Selecting it will open the tasks.json file. Delete the script displayed and replace it by the following:

{
    "version": "0.1.0",
    "command": "chrome",    
    "windows": {
        "command": "chrome.exe"
    },
    "args": ["basicJavascript.html"]
}
Remember to change the "args" section of the tasks.json file to the name of your file. This will always open that specific file when you hit F5.

You may also set the this to open whichever file you have open at the time by using ["${file}"] as the value for "args". Note that the $ goes outside the {...}, so ["{$file}"] is incorrect.

Save the file.

Switch back to your html file (in this example it's "text.html"), and press ctrl + shift + b to view your page in your Web Browser.
