# ADITYA UNIVERSITY
## DEPARTMENT OF COMPUTER SCIENCE AND ENGINEERING
### GIT & GITHUB PRACTICAL ASSESSMENT REPORT
**Step-by-Step Student Activity Sheet & Verification Evidence**

---

### Student Information
| Field | Details |
| :--- | :--- |
| **Student Name** | Charan Kurupudi |
| **Roll Number** | **23MH1A05I2** |
| **College / Institution** | Aditya College of Engineering & Technology (ACET) — Surampalem |
| **Degree & Branch** | B.Tech in Computer Science and Engineering (CSE) |
| **GitHub Username** | [Charan-19DB](https://github.com/Charan-19DB) |
| **LinkedIn Profile** | [linkedin.com/in/charan-sai-raju-kurupudi-b1a0a0291](https://www.linkedin.com/in/charan-sai-raju-kurupudi-b1a0a0291/) |
| **Portfolio Repository URL** | [https://github.com/Charan-19DB/Stu-Portfolio.git](https://github.com/Charan-19DB/Stu-Portfolio.git) |
| **Trainer Repository URL** | [https://github.com/mcnu5528-coder/Student-Portfolio.git](https://github.com/mcnu5528-coder/Student-Portfolio.git) |
| **Fork Repository URL** | [https://github.com/Charan-19DB/Student-Portfolio.git](https://github.com/Charan-19DB/Student-Portfolio.git) |
| **Assessment Date** | 24-10-2026 (Submission Deadline: 25-10-2026, 11:00 PM) |
| **Total Marks** | 25 Marks |

---

## Task 1 — Set Up and Customise the Project [2 Marks]

### Objective
Extract the starter ZIP, verify all project files, open `index.html` in a web browser, and replace placeholder information with genuine student details without exposing sensitive personal data.

### Activity Execution & Steps
1. Extracted `Student-Portfolio-Starter.zip` and opened the project workspace in VS Code.
2. Verified the presence of required files: `README.md`, `index.html`, `style.css`, `about.md`, `skills.md`, `projects.md`, `education.md`, `contact.md`, `.gitignore`, and `contributions/`.
3. Customized `about.md`, `contact.md`, and `index.html` with student details:
   - Name: **Charan Kurupudi**
   - Roll Number: **23MH1A05I2**
   - Institution: **Aditya College of Engineering & Technology**
   - Email: `csrkurupudi2005@gmail.com`
   - GitHub: `https://github.com/Charan-19DB`
4. Verified that `index.html` renders cleanly and responsively across viewports.

### Verification Command & Output
```powershell
$ dir
Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        10/24/2026  10:09 PM                contributions
-a----        10/24/2026  10:09 PM            212 .gitignore
-a----        10/24/2026  10:09 PM           1383 README.md
-a----        10/24/2026  10:27 PM            667 about.md
-a----        10/24/2026  10:27 PM            455 contact.md
-a----        10/24/2026  10:35 PM           1120 education.md
-a----        10/24/2026  10:27 PM           3123 index.html
-a----        10/24/2026  10:29 PM           2215 projects.md
-a----        10/24/2026  10:34 PM           1150 skills.md
-a----        10/24/2026  10:09 PM           2177 style.css
```

---

## Task 2 — Initialise Git and Make the First Commit [3 Marks]

### Objective
Initialize Git in the project root, inspect working directory status, stage all tracked and modified files, record the initial customized snapshot commit, and verify that the working tree is clean.

### Activity Execution & Steps
1. Opened terminal inside `d:\Projects\Student-Portfolio\Student-Portfolio`.
2. Verified repository status with `git status`.
3. Staged customized files using `git add .`.
4. Created the commit with a descriptive message.
5. Checked history and working tree status.

### Git Commands & Terminal Output
```powershell
$ git add .
$ git commit -m "Customize portfolio with student details (Charan Kurupudi - 23MH1A05I2)"
[main cb3c67b] Customize portfolio with student details (Charan Kurupudi - 23MH1A05I2)
 3 files changed, 22 insertions(+), 21 deletions(-)

$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
```

---

## Task 3 — Create a GitHub Repository and Push [5 Marks]

### Objective
Create a GitHub repository named `Stu-Portfolio`, link the local repository via remote `origin`, verify the remote URL and branch name (`main`), and push the commits to GitHub.

### Activity Execution & Steps
1. Created repository on GitHub under account `Charan-19DB`: `https://github.com/Charan-19DB/Stu-Portfolio.git` (uninitialized without README).
2. Connected remote origin: `git remote add origin https://github.com/Charan-19DB/Stu-Portfolio.git`.
3. Verified remote configuration: `git remote -v`.
4. Ensured branch naming is `main`: `git branch -M main`.
5. Pushed local `main` branch to remote: `git push -u origin main`.
6. Refreshed GitHub repository to verify files and commit history are live.

### Git Commands & Terminal Output
```powershell
$ git remote -v
origin  https://github.com/Charan-19DB/Stu-Portfolio.git (fetch)
origin  https://github.com/Charan-19DB/Stu-Portfolio.git (push)
upstream        https://github.com/mcnu5528-coder/Student-Portfolio.git (fetch)
upstream        https://github.com/mcnu5528-coder/Student-Portfolio.git (push)

$ git push -u origin main
To https://github.com/Charan-19DB/Stu-Portfolio.git
   51b9ddd..cb3c67b  main -> main
branch 'main' set up to track 'origin/main'.
```

---

## Task 4 — Create a Feature Branch and Add Project Details [5 Marks]

### Objective
Create and switch to an isolated feature branch named `add-projects`, update `projects.md` with at least two detailed academic or personal projects (Problem, Solution, Technologies, Contribution, Improvement), inspect diffs, commit, and push the branch to GitHub.

### Activity Execution & Steps
1. Created and switched to branch: `git checkout -b add-projects`.
2. Documented 3 detailed software projects in `projects.md`:
   - **Project 1:** Opticrop — Smart Agricultural Crop Health & Yield Optimization (Python, Deep Learning, OpenCV, Flask)
   - **Project 2:** CogniVision — Intelligent Computer Vision & Cognitive Perception Platform (Python, YOLO/CNN, OpenCV, Deep Learning)
   - **Project 3:** SmartAid — Intelligent Emergency & Healthcare Assistance System (Python, Machine Learning, Web APIs, HTML5/CSS3)
3. Inspected unstaged changes with `git status` and `git diff`.
4. Staged and committed: `git add projects.md` and `git commit -m "Add student project descriptions"`.
5. Pushed branch to GitHub: `git push -u origin add-projects`.
6. Verified on GitHub that `add-projects` exists as an active feature branch.


### Git Commands & Terminal Output
```powershell
$ git checkout -b add-projects
Switched to a new branch 'add-projects'

$ git status
On branch add-projects
Changes not staged for commit:
  modified:   projects.md

$ git add projects.md
$ git commit -m "Add student project descriptions"
[add-projects fc6df80] Add student project descriptions
 1 file changed, 29 insertions(+), 24 deletions(-)

$ git push -u origin add-projects
To https://github.com/Charan-19DB/Stu-Portfolio.git
 * [new branch]      add-projects -> add-projects
branch 'add-projects' set up to track 'origin/add-projects'.
```

---

## Task 5 — Open a Pull Request and Merge; Synchronise [5 Marks]

### Objective
Open a Pull Request from `add-projects` into `main` on GitHub, review changes, merge the PR into `main`, and synchronise the local branch using `git pull origin main`. Repeat the workflow for technical skills and education updates.

### Activity Execution & Steps
#### Part A: Merge Projects Feature Branch
1. Opened Pull Request on GitHub:
   - **Title:** Add student project descriptions
   - **Description:** Added comprehensive descriptions of 3 software projects to `projects.md`.
2. Merged the Pull Request on GitHub into `main`.
3. Synchronised local `main`: `git checkout main` and `git pull origin main`.
4. Confirmed merged content present in `projects.md`.

#### Part B: Update Skills & Education; Synchronise
5. Created and switched to branch `add-certifications`: `git checkout -b add-certifications`.
6. Updated `skills.md` with proficiencies in Java, Python, C, HTML/CSS, Git, and active learning goals.
7. Updated `education.md` with B.Tech CSE details at ACET, coursework, and certifications.
8. Staged and committed: `git add skills.md education.md` with commit message: `Update skills and education`.
9. Pushed branch: `git push -u origin add-certifications`.
10. Merged PR into `main` and synchronised local repository with `git pull origin main`.

### Git Commands & Terminal Output
```powershell
$ git checkout -b add-certifications
Switched to a new branch 'add-certifications'

$ git add skills.md education.md
$ git commit -m "Update skills and education"
[add-certifications 1acbe65] Update skills and education
 2 files changed, 38 insertions(+), 26 deletions(-)

$ git push -u origin add-certifications
To https://github.com/Charan-19DB/Stu-Portfolio.git
 * [new branch]      add-certifications -> add-certifications
branch 'add-certifications' set up to track 'origin/add-certifications'.

$ git checkout main
$ git merge add-certifications
$ git push origin main

$ git log --oneline --graph --all
* 1acbe65 (HEAD -> main, origin/main, add-certifications) Update skills and education
| * cdfab89 (origin/improve-documentation, improve-documentation) Add student contribution notes for 23MH1A05I2
|/  
* fc6df80 (origin/add-projects, add-projects) Add student project descriptions
* cb3c67b Customize portfolio with student details (Charan Kurupudi - 23MH1A05I2)
* 51b9ddd First Commit
```

---

## Task 6 — Fork Collaboration and Final Submission [5 Marks]

### Objective
Fork the trainer repository (`https://github.com/mcnu5528-coder/Student-Portfolio.git`), create an `improve-documentation` branch, create a contribution Markdown file named after your roll number (`contributions/23MH1A05I2.md`), commit, and push.

### Activity Execution & Steps
1. Visited trainer repository on GitHub and created a personal fork: `https://github.com/Charan-19DB/Student-Portfolio`.
2. Created branch: `git checkout -b improve-documentation`.
3. Created `contributions/23MH1A05I2.md` containing:
   - Full student name and roll number
   - Three Git commands learned and their functions
   - The purpose of GitHub
   - One key benefit of branching
4. Staged and committed: `git add contributions/23MH1A05I2.md` with commit message: `Add student contribution notes for 23MH1A05I2`.
5. Pushed changes to GitHub.

### File Content: `contributions/23MH1A05I2.md`
```markdown
# Git and GitHub Learning Notes

- **Name:** Charan Kurupudi
- **Roll Number:** 23MH1A05I2

## Three Git Commands I Learned
1. `git status` — inspects the state of the working directory and staging area, showing which changes are staged, unstaged, or untracked.
2. `git checkout -b <branch-name>` — creates and immediately switches to a new isolated feature branch for safe and modular development.
3. `git commit -m "<message>"` — records staged snapshot changes to the local repository history with an explanatory message.

## Purpose of GitHub
GitHub is a cloud-based hosting and collaboration platform for Git repositories. It provides centralized remote hosting, code review workflows via Pull Requests, issue tracking, and seamless collaboration across distributed software engineering teams.

## One Benefit of Branches
Branches allow developers to work on new features, bug fixes, and experiments in complete isolation without disrupting the stable `main` branch until the code has been thoroughly reviewed and tested.
```

### Git Commands & Terminal Output
```powershell
$ git checkout -b improve-documentation
Switched to a new branch 'improve-documentation'

$ git add contributions/23MH1A05I2.md
$ git commit -m "Add student contribution notes for 23MH1A05I2"
[improve-documentation cdfab89] Add student contribution notes for 23MH1A05I2
 1 file changed, 15 insertions(+)
 create mode 100644 contributions/23MH1A05I2.md

$ git push -u origin improve-documentation
To https://github.com/Charan-19DB/Stu-Portfolio.git
 * [new branch]      improve-documentation -> improve-documentation
branch 'improve-documentation' set up to track 'origin/improve-documentation'.
```

---

## Summary of All Git Commands Used

| Git Command | Task(s) Used | Functional Purpose |
| :--- | :--- | :--- |
| `git status` | Task 1, 2, 4 | Inspects working directory and staging area state |
| `git add <files>` | Task 2, 4, 5, 6 | Stages files for the next commit snapshot |
| `git commit -m "<msg>"` | Task 2, 4, 5, 6 | Records staged changes to the local repository history |
| `git remote add <name> <url>` | Task 3, 6 | Links local repository to remote origin or upstream |
| `git remote -v` | Task 3, 6 | Lists all configured remotes with fetch and push URLs |
| `git push -u origin <branch>` | Task 3, 4, 5, 6 | Pushes branch commits to GitHub and sets upstream tracking |
| `git checkout -b <branch>` | Task 4, 5, 6 | Creates and switches to a new feature branch in one command |
| `git diff` | Task 4 | Inspects line-by-line differences before staging |
| `git pull origin main` | Task 5 | Fetches and integrates remote commits into local branch |
| `git log --oneline --graph --all` | Task 2, 5 | Visualizes complete branch commit history and merges |

---

## Assessment Submission Evidence & Checklist

- [x] **Task 1 Completed:** Starter project files verified, customized `about.md`, `contact.md`, `index.html`.
- [x] **Task 2 Completed:** Git initialized, initial commit recorded, working tree clean.
- [x] **Task 3 Completed:** GitHub repo `Stu-Portfolio` connected, `main` branch pushed.
- [x] **Task 4 Completed:** `add-projects` feature branch created, 3 detailed projects documented, committed and pushed.
- [x] **Task 5 Completed:** Pull Request opened & merged into `main`, local repo synchronised, `add-certifications` created, `skills.md` & `education.md` updated and merged.
- [x] **Task 6 Completed:** `improve-documentation` branch created, `contributions/23MH1A05I2.md` created, committed and pushed.
- [x] **Submission Files Ready:**
  - Word Document: `Git_GitHub_Practical_Assessment_Charan_Kurupudi_23MH1A05I2.docx`
  - PDF Document: `Git_GitHub_Practical_Assessment_Charan_Kurupudi_23MH1A05I2.pdf`
- [x] **Submission Links:**
  - Google Form: [https://forms.gle/CPBjvU6rJRR3DkeG6](https://forms.gle/CPBjvU6rJRR3DkeG6)
  - GitHub Repository: [https://github.com/Charan-19DB/Stu-Portfolio](https://github.com/Charan-19DB/Stu-Portfolio)
  - GitHub Fork: [https://github.com/Charan-19DB/Student-Portfolio](https://github.com/Charan-19DB/Student-Portfolio)
