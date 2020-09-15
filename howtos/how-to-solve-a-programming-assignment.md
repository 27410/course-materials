# How to solve a programming assignment (from A to Z)

Step-by-step:
1. Paste the assignment URL into your browser.
2. Accept the assignment on GitHub Classroom.
3. GitHub classrom will create an assignment repository specifcally for you (`assignment-name-your-GitHub-username`). Click on the created link to navigate to that repository on GitHub.
4. Copy the repository URL (big green "Code" button in the menu) and navigate to [class27410.bioengineering.dtu.dk](https://class27410.bioengineering.dtu.dk/).
5. Open a terminal using the + icon in the JupyterLab menu.
6. Execute `git clone PUT-YOUR-REPOSITORY-URL-HERE` to clone a local version of the assignment repository onto the DTU JupyterLab.
7. Using the JupyterLab file browser, navigate inside the repository and double click the `README.md` file.
8. Thoroughly read the assignment information in `README.md`.
9. Double click the `assignment.py` file to get an overview of how and where to put your solutions to the assignment.
10. Click the + icon to open a Jupyter Notebook[1] (Python 3) to iteratively develop solutions to the assignment.
11. Once you developed a solution to a task in the assignment, copy-paste the code into the suggested spot in  `assignment.py`.
12. Open a terminal (+ icon in menu) and navigate inside the top-level of the assignment directory. If you don't know how to do this, read "How to use the commandline".
13. OPTIONAL: you can run `pytest assignment.py`[2] in a terminal to run the same test suite that GitHub classroom to assess your solutions before submitting them.
14. Run `git status` to see what files have changed since the last commit (if you don't know what a commit is, read "How to use git and GitHub"). `assignment.py` and potentially other files that you have either created or modified should be highlighted here.
15. Run `git add .` to stage all modified files to be committed (the `.` means the current directory).
16. Commit the file and leave a commit message by running `git commit -m "PUT YOUR MESSAGE HERE."`.
17. Push the changes to GitHub by running `git push`
18. Navigate to GitHub and click on the "Actions" button in the menu. Click on your latest commit to see if the tests passed and you solved the assignment. If not got, return to your Jupyter notebook in step 10 (rinse and repeat). Otherwise, congratulations!

[1] It is recommended to use a Jupyter notebook to develop a solution because it is easy to see intermediate results etc.
[2] You might have to install `pytest` first by running `pip install pytest` in a terminal (which you can open with the + icon in the menu). Furthermore, you will have to 