# Distributed Configuration Files

Installation
==

Put a `config` directory in your home directory, and make a git repository in `config/src`. Clone this repo into `config/tools`, and use the tools to export and link your existing configuration files to the new repo. You can then clone `config/src` and `config/tools` on any machine you like, and use the `link` tool to sync your local configuration on that machine with the repo copy, or `import` to simply copy the files without syncing.


Silly Advertisement
==

Sync your shell and editor settings over multiple computers!!
-
Just replace your config files with symlinks to the files in your repo; it's that easy!
No more carting around USBs full of old and new rc files! Once you've made a clever change to one of your rc files, just `commit` and `push`! Then, `pull` it to any of your other computers that could benefit from that change!

Scripts to easily update and link files!!
-
Use `export` to update the repository with unlinked local files, overwriting existing files  
Use `link` to link you local files with the repository, overwriting local originals  
Use `import` to update the local files with files from the repo, overwriting links  

Misc
==

Git doesn't track repositories inside other repositories unless you tell it to specifically.  
Use the `git submodule` set of commands. I'm not too familiar with it myself, but `git submodule add <url>` clones the repository, and tracks it.
