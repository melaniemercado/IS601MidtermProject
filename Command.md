# Command Line Tutorial 

<center>**What is the Command Line?**</center>

- The **Command line** is a *text interface for your computer.* It's a program that takes in commands, which it passes on the computer's operating system to run. 

<center>**What do you do to use it?**</center>

- From the command line, you can navigate through **files** and **folders** on your computer, just as you would like your Windows Explorer on Windows or Finder on MAC OS. The Difference is that the **command line is fully text-based**. 

<center>**How do you use it?**</center>

- In order to use the command line, one has to understand the various commands. In order to access the command line, you have to use your *terminal*. The terminal is where you would use the commands that will be explained later in the tutorial. Below is an example of what the terminal could look like. 

![](https://lh3.googleusercontent.com/UMl_LOhLP3WklhOXK0-RfWzC0_yAw7Jid0HcN3V0F26besFzsvGPgcZdGOwpopECjw8QPMEpGwk)


# VI 
-**vi** is a screen-oriented text editor originally created for the Unix operating system. The portable subset of the behavior of vi and programs based on it, and the text  editor language supported within these programs, is described by (and thus standardized by) the [Single Unix Specification.

To edit open a file using Vi, simply type in vi "filename.md" 

![](https://lh3.googleusercontent.com/aZ9vt3BaVMGaioRaFdTvQioKFjAhiTn5YTm4w4HglWwcDfcw-oAkZOSj8frGKgIa6GTok9Cbx_s)

Then press 'I' to enable to text editor

![](https://lh3.googleusercontent.com/cyXJZGsFmWEW-GbH5XqFDzsC3XrLXaXacrY5BxMNfgFPlGXI_UUb9QpvPCzf38j2snv2j9hYT_Y)

Once you're done with your edits, press the **esc**, then *shift + :*, this will allow you to type **wq** which will save and close the file. 

![enter image description here](https://lh3.googleusercontent.com/GAxFdo2-NkdLdmlJ9pYRdjNn1ECV4ebDPHjaWGJdZrGiGiGyqw3kKXryDnhjWZme7EF7WTsoits)

*Thats how you use VI!*


# Commands

<center>**CD: Change Directory**</center>

-  **CD** takes a directory name as an *argument*, and switches into that directory. To navigate directly to a directory, use cd with the directory's path. 

This is how the user would type out the cd command.
![](https://lh3.googleusercontent.com/_RvDc12BRvqAFNf9Z4xXxRL7ff9qYYTdsZIwqSJHOWpCNNgzqj2XeoWZfC8Z_X6Cx-zEGps_WHs)

- This example shows the user switching into the desktop directory. By simply typing 'CD' and then the directory name, you will find yourself in that directory.

<center>What if the user wanted to **go back to a previous directory?**</center>

- To go **back** to a previous directory, the user would have to use the **'cd . .'** command.
![](https://lh3.googleusercontent.com/Ipe9KEb7jEVsbX7gkjmtuTAu6UNX997BbS-qIhE2fUws-qerNtp4P2GU8ZggXA_nb_lhsEid_84)

> By simply using the **. .** at the end of the cd command, the user is able to go back to the previous directory they were working on.

<center>**MKDIR: Make Directory**</center>

- mkdir takes in a directory name as an argument, and then creates a new directory in the current working directory. Here we use mkdir to create a new directory named my_folder.

![](https://lh3.googleusercontent.com/34TUZFlCxuJen9pImaStzibxjqai2L6ctT7LbpRMuRfG8OqE7MLUSBgQC_VK6V2AtwIyp2Az3u8)

- To confirm that the directory was created, list out all the directories. my_folder appears as a directory after it was created.

![](https://lh3.googleusercontent.com/UD3KAUSwneWerKpy93bWbVbQZyxPpBMvG3z_FEbr_v4SuIIG3fzMseUredmoa_yVNl1O6h-6Qug)



<center>**CP: Copy**</center>


- cp copies files or directories. It can be used when you want to copy an image, or files into another location.

![](https://lh3.googleusercontent.com/_aZrFdE8saPIur72c-4FdOftahh-gtbwtaZX_P9ookw-mGdUeKOSWuGDU2XeNWch-sPWPIdgKNQ)

<center>**PWD:  Print Working Directory**</center>
- pwd prints the name of the working directory. This will allow you to always know what directory you are working in if you ever forget.

![](https://lh3.googleusercontent.com/lvqGdMFOlUL6gr7LG81yXNEWIWBEu_fIcYaD7mAwLZvutBGng9BCM90lh0pzZb4aksyEXTwvaAk)



<center>**MV: Move File or Directory**</center>

* The mv command allows you to move one file from one directory into another. To move a file into a directory, use mv with the source file as the first argument and destination directory as the second argument.

![](https://lh3.googleusercontent.com/SJtZvaheRfpkNEk0V9yJV-glUWzxMT1kwE2-CyHq5HTeZj6DYS5bOzyUzhTRklytaQVw5A9hvjU)


<center>**RM: Remove**</center>

- The **rm** command is when you want to delete a file. This could be used when you no longer need a file or image.

![](https://lh3.googleusercontent.com/90yEzwYotZzyH59OxiIwZCxW3jKEogexBoVCLIv6h5m_KK414j8I47NejRVXxWaDIsniHW9scqY)

<center>**History**</center>

- In its most simple form, you can run the ‘history’ command by itself and it will simply print out the bash history of the current user to the screen. Commands are numbered, with older commands at the top and newer commands at the bottom.

![](https://lh3.googleusercontent.com/f8C6ss1KanuLDF8PJjLZtCdszSsDgfYFvt2buaAC6h6-HMFgJh22v5l84OTkZTyS3Nj3IPXb-hY)


<center>**Home Directory and '~'**</center>

- A **home directory** is a file system directory on a multi-user operating system containing files for a given user of the system. The specifics of the home directory (such as its name and location) are defined by the operating system involved; for example, Linuxhome/*username* and Windows systems between 2000 and Server 2003 keep home directories in a folder called Documents and Settings

- **~** (_tilde_) is an alias for **home** directory.
> Below is an example of the Home Directory 

![](https://lh3.googleusercontent.com/MZk_xav5aUQIs8E7MQvWh338MVEOIRsgnw6eekstU5hgHt0O5V5rvgKeQJY61fw74fxfaqjnD9M)

<center>**File Paths in Linux**</center>

- A file path is the human-readable representation of a file or folder’s location on a computer system. You’ve seen file paths, although you may not realize it, on the internet: An internet URL, despite ancient battles fought by proprietary companies like AOL and CompuServe, is actually just a path to a (sometimes dynamically created) file on someone else’s computer. For instance, when you navigate to example.com/index.html, you are actually viewing the HTML file index.html, probably located in the **var** directory on the example.com server. Files on your computer have file paths, too, and this article explains how to understand them, and why they’re important.

> The highlighted portion on this terminal is an example of a *file path*

![enter image description here](https://lh3.googleusercontent.com/IN9zDgWDUpR_FrTiBzT951PYYdtLjbVaOXvwAJZa6P8wbL5ohQVWbM2orecYh-B5fjPonc4ejYk)
  

<center>**Using the tab key to complete file paths**</center>

- Usually in a Unix/Linux terminal when you press tab it will autocomplete with several options and then it will list the options below for you to select. This is a great feature if you spend a lot of time in the terminal. **However, you have to enable it.** 

> Below are the steps to enable auto-complete file paths for mac. 

![](https://lh3.googleusercontent.com/1a500nlZxO4iRw64TpApbdPtPtWJbtiabVDLy22C0-jK_fD7wrj4LR7k-EJj5DQmofmXOkYg1yc)


<center>**Using Up and Down Arrows for History**</center>

-  The Terminal tracks your command history—that is, it keeps a record of the commands you’ve used, and you can scroll through those historical commands. **Press the Up Arrow key from the command prompt, and you’ll see the most-recently used command**; each additional press moves further back through history, and the **Down Arrow key moves forward in the history file.**

> below you'll see what the terminal looks like before the Up arrow is selected. 

![](https://lh3.googleusercontent.com/KH1T593u0GzBPTzoD81U4ANTed4ISsEkRg-nyT2V8bWlO4HtTFHd6r77kIfxlGTA7Bvn1I7K9VQ)

>Below you'll see that pressing the Up arrow will bring the last typed out command. 

![](https://lh3.googleusercontent.com/KrDEbS8VDEUQ7bpdq4iAkwKp_54Hv8A9-ojTwnUSJqnDxtVmWC_QgmE15ug5Gj8NZap7mwEEt6k)

