Important things to note:
- When making changes to a file, always create a new branch and git pull beforehand to make sure you are up-to-date.
- Whenever you commit a change, always submit a pull request before reopening a branch and submitting an additional commit to avoid merge conflicts (Eilidh you know what you did).
- For file naming conventions, allowed characters are: a-z (lowercase), 0-9, and _

File naming conventions:

Why no spaces allowed? When using CLIs (Command Line Interface), [name example] is read by CLIs as two separate files, i.e, [name] [example]. Either have it all one word [nameexample], or use underscores, [name_example].

Why only lowercase? Granted, everyone in the group is using Windows as their OS. However, if anyone were to use Linux, for example, [Nameexample] and [nameexample] would be read as two completely different files, compared to Windows, which read them as the same. Not the end of the world, but it's good practice.

Please, for the love of everything, DO NOT use special characters. The biggest offenders are: & * /    These are used to run commands, and if are included in file names, if you don't surround them with hard quotes ['example'] it WILL cause issues.

How to make changes (Using a CLI):
1. Clone the repo - git clone <url>
2. Make sure it's up to date (every time) - cd into the directory and run: git pull
3. Create new branch: git switch -c <branch_name>
4. Get the repo to track your branch: git push --set-upstream origin <branch_name>
5. Add the files into your branch: git add <file_name>
7. Check your files are being tracked: git status
8. Make sure all files are included properly and status is green
9. Commit your changes to the branch: git commit -m "<commit message that explains what you've done>"
10. Create a pull request: git pull
