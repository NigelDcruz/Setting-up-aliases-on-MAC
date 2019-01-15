
# Setting up (Git) aliases on MAC

## .bash_profile

In case you're not aware, there's a hidden file in your Mac’s user directory named as **.bash_profile**. This file mostly allows you to configure your command line interface the way you need it. Basically, you can change the terminal prompt, colors of text, **add aliases to functions you use all the time**, and so much more.

You should know right now that this file has a '.' at the beginning of its name which makes it invisible. So you won't be able to find it in your Mac's Finder. To view invisible files in the Terminal you can use the following command:
```
ls -al
```

## Setting up aliases

### Step 1

- Navigate to the User Directory where the **.bash_profile** file is located. 
  Type:
  ```
  ~/.bash_profile
  ```
  
### Step 2

Open the **.bash_profile** file using the following command:
```
nano .bash_profile
```
- This command will open the .bash_profile document (or create it if it doesn’t already exist) in the Nano text editor.

### Step 3

Use the following command to create the alias:
```
alias gs='git status' 
```
- So whenever you type **gs** in your terminal, it will be replaced by **git status**.
- You can change the name (**gs**) to anything you'd like.
- Let's create aliases for some of the basic Git commands

```
alias gs='git status'
alias ga='git add .'
alias gc='git commit -m'
alias gpom='git pull origin master'
alias gpm='git push origin master'

```

### Step 4 

- To Save the changes, press **ctrl**+**o** and then press **Enter** (Return).
- Next, press **ctrl**+**x** to Exit.

### Step 5
- Note: If we're making any changes to the **.bash_profile** file, we need to compile the file.
- To that, we just type:
```
source ~/.bash_profile
```

That's it, you can start using the aliases now. Similarly, you can create aliases for anything you want.
