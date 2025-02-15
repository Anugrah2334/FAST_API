# Version Control Systems

## Subversion (SVN)

Subversion (SVN) is an open-source version control system that allows users to track changes, revert to previous versions, and merge new features efficiently.

### Types of Version Control Systems:
- **Centralized Version Control System (CVCS):** A single central server stores all versions.
- **Distributed Version Control System (DVCS):** Each user has a full copy of the repository.

### Why Use Version Control?
- Track all changes and maintain history.
- Rollback to previous versions when necessary.
- Merge new features seamlessly.

### Installing & Setting Up SVN on Windows:
1. Download and install SVN (TortoiseSVN).
2. Restart your system after installation.
3. Verify the installation using:

   ```sh
   svn --version
   ```
![Example Image](https://github.com/Anugrah2334/Devops-Assignment/blob/main/Screenshot1.jpg)

### SVN Commands
#### Step 1: Initialize the Repository
```sh
svnadmin create ~/svn_repo/my_project
```
![Example Image](https://github.com/Anugrah2334/Devops-Assignment/blob/main/Screenshot2.jpg)

#### Step 2: Checkout the Repository
```sh
svn checkout file:///path/to/svn_repo/my_project
```
![Example Image](https://github.com/Anugrah2334/Devops-Assignment/blob/main/Screenshot3.jpg)

#### Step 3: Add Files to the Directory
```sh
cd my_project
svn add file.txt
svn commit -m "Added file.txt"
```
![Example Image](https://github.com/Anugrah2334/Devops-Assignment/blob/main/Screenshot4.jpg)
![Example Image](https://github.com/Anugrah2334/Devops-Assignment/blob/main/Screenshot5.jpg)

#### Step 4: Update Your Working Copy and View Logs
```sh
svn update
svn log
```
![Example Image](https://github.com/Anugrah2334/Devops-Assignment/blob/main/Screenshot6.jpg)

#### Step 5: Reverting Changes
```sh
svn revert file.txt
```
![Example Image](https://github.com/Anugrah2334/Devops-Assignment/blob/main/Screenshot7.jpg)

#### Step 6: Creating a Branch and Merging Changes
```sh
svn copy file:///C:/svn_repos/my_repo/trunk file:///C:/svn_repos/my_repo/branches/feature-branch -m "Creating feature branch"
svn merge file:///C:/svn_repos/my_repo/branches/feature-branch
```

---
![Example Image](https://github.com/Anugrah2334/Devops-Assignment/blob/main/Screenshot8.jpg)

## Mercurial (Hg)

Mercurial is a distributed version control system (DVCS) designed for efficient handling of projects of all sizes. It is similar to Git but focuses on simplicity and ease of use. Written in Python, it is known for its intuitive commands, robust performance, and cross-platform compatibility.

### Features of Mercurial:
- **Distributed Version Control:** Each developer has a full copy of the repository, enabling offline work and independent branching.
- **Lightweight and Fast:** Efficiently handles large projects and binary files.
- **Cross-Platform:** Works on Windows, macOS, and Linux.
- **Extensible:** Supports plugins for additional functionality.
- **Simple and Intuitive Commands:** Consistent syntax and easy to learn.

### Installing & Setting Up Mercurial on Windows:
1. Download and install Mercurial (TortoiseHg).
2. Restart your system after installation.
3. Verify the installation using:

   ```sh
   hg --version
   ```
   ![Example Image](https://github.com/Anugrah2334/Devops-Assignment/blob/main/Screenshot9.jpg)

### Mercurial Commands
#### Step 1: Creating and Initializing the Repository
```sh
hg init my-hg-repo
```
![Example Image](https://github.com/Anugrah2334/Devops-Assignment/blob/main/Screenshot10.jpg)

#### Step 2: Adding and Committing Files
```sh
hg add file.txt
hg commit -m "Added newfile.txt"
```
![Example Image](https://github.com/Anugrah2334/Devops-Assignment/blob/main/Screenshot11.jpg)
![Example Image](https://github.com/Anugrah2334/Devops-Assignment/blob/main/Screensho12.jpg)
#### Step 3: Cloning, Updating, and Reverting
```sh
hg clone https://example.com/repo
hg pull
hg update
hg log
```
![Example Image](https://github.com/Anugrah2334/Devops-Assignment/blob/main/Screenshot13.jpg)

#### Step 4: Branching and Merging
```sh
hg branch new-feature
hg merge
```
![Example Image](https://github.com/Anugrah2334/Devops-Assignment/blob/main/Screenshot14.jpg)