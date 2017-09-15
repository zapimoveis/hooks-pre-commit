# hooks-pre-commit
Pre-commit GIT hook for validate ZAP standard/rules commit

Before starting to contribute in any of library that is on this github is necessary to setup the pre-commit hook.

**Note: If you don't install this pre-commit you may have your pull request denied because of some out of standard code (like forget some AWS Key or Secret Key in your code).**

## Setup
<ol>
<li>
Clone the repository you will work
</li>
<li>
In your command line enable git templates (in the folder of the repo):

```
git config init.templatedir '~/.git-templates'
```

This tells git to copy everything in ~/.git-templates to your per-project .git/ directory when you run git init

</li>
<li>
Create a directory to hold the global hooks:

```
mkdir -p ~/.git-templates/hooks  
```

**Note: in windows your root directory will be something like c:\user\.git-templates**

</li>
<li>
Copy the ZAP hook standard file into your local folder (~/.git-templates/hooks).
</li>
<li>
Re-initialize git in each existing repo you'd like to use this in:

```
git init
```

**Note: It will not overwrite anything**

</li>
</ol>