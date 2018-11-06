AberSailbot - Git Workshop
==========================

This workshop will familiarise you with using git, and the reason for its use in version control.

You should first copy this repository so that you have your own version to work on for the time being.

On GitHub, you will see a "Fork" button on the top right hand side. You should fork this repository into your own account. This simply creates an exact copy on your own account that you have permission to work on.

Ensure that you are now in your own "Fork" of the repository (you should see YOURUSERNAME/git-workshop at the top of the page.

To get a local copy of this repository (called "cloning" in git terms), run the following in a terminal:

    $ git clone https://github.com/YOURUSERNAME/git-workshop
    $ cd git-workshop/

You can now try running the (somewhat useless) python code:

    $ python3 my_name.py

Change the string in my\_name.py to something different (like your own real name) so that you get a different result when you run it.

You now want to let git know that you've changed something in the code. In order to do this, you need to tell git which file has changed with:

    $ git add my_name.py

OPTIONALLY, if you'd like to see the changes git has now detected, you can run:

    $ git diff --cached

Your changes have now been added to something similar to a staging area, ready to be
committed. In other words, you can now say that you want to make a note of the changes you have made and told git about.

This should be done with a `commit`:

    $ git commit

A text editor should appear, in which you should add a message to your commit. Should you end up in the vi/vim text editor, see the bottom of this README for some handy shortcuts.

This message should describe briefly what the commit is, and why it was made.
This may be a description of a newly added feature, or a change to your existing code.
Your commit to this repository is simple and the purpose is known, so a short
message such as `Change name to my own` will suffice.

When you're ready to "upload" this commit to the central repository (from your
local copy), you can run:

    $ git push

If you want to get the latest changes made by someone else from a remote repository, run:

    $ git pull

Vi/Vim Shortcuts
----------------

Whenever you want to run any commands in vi, press escape before doing so. This allows you to give commands. You can then use the following:

i - Press i in order to be able to start typing text at your current cursor position
:q - Quit without saving changes
:wq - Save your changes and quit

