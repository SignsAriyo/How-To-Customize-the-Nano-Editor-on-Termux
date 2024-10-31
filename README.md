# How-To-Customize-the-Nano-Editor-on-Termux

#Here are the six amazing things you didn't know you can achieve with the Nano Code Editor on the Termux app

_Nano allows customization, and am not talking about just changing the theme from light to dark, but you can do whatever you imagine_

Imagine you can now have line numbers, new color for the syntax texts, you can have a touch mouse(no more using the arror keys on the keyboard to move the cursor) and set an auto-indentation 

##Here is the process

After you must have updated Termux with `apt update && apt upgrade` and installed nano with ,`apt install nano`, check if nano has been installed with `nano --version` _(a set of numbers should appear, if its doesn't then nano wasn't installed successfully)_

Next, we need to edit nano by opening a hidden file called the nanorc with **(Make sure you are in the default working directory, make sure you `cd` before moving to this step)**

```bash
nano ~/.nanorc
```

remember, because nanorc is a hidden file, that's why we have the . in front of nanorc

Once, you are inside the file, paste this prompts

```bash
set softwrap
set linenumbers
set tabsize 4
set mouse
set autoindent
```
#Image

This is what the nanorc file should look like
![image of the nanorc file](https://imgur.com/a/nanorc-jEtL8DO, "nanorc")

Then, press `Ctrl+O` to save and `Ctrl+X` to close nano

Now, test it and enjoy

#RESULT 
![new nano code editor interface](https://i.imgur.com/7LmXaPr.jpeg,"nano_editor")

#COMMENTS:
1. set softwrap makes your code collapsible, and easily move to the next line
2. set linenumbers numbers the lines
3. set tabsize 4 gives you a definite tab space, so you can avoid errors especially if you are a Python dev
4. set mouse gives you the ability to tap anywhere while you are in nano}
5. set autoindent adds indentation automatically}
