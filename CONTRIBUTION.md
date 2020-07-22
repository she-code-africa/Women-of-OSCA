# WOSCA Contribution guidelines

## Fork this repository

Fork this repository by clicking on the fork button on the top of this page.
This will create a copy of this repository in your account.

## Clone the repository

Now clone the forked repository to your machine. Go to your GitHub account, open the forked repository, click on the clone button and then click the *copy to clipboard* icon.

Open a terminal and run the following git command:

```
git clone "url you just copied"
```
where "url you just copied" (without the quotation marks) is the url to this repository (your fork of this project). See the previous steps to obtain the url.

For example:
```
git clone https://github.com/this-is-you/Women-of-OSCA.git
```
where `this-is-you` is your GitHub username. Here you're copying the contents of the Women-of-OSCA repository on GitHub to your computer.

## Create a branch

Change to the repository directory on your computer (if you are not already there):

```
cd Women-of-OSCA
```
Now create a branch using the `git checkout` command:
```
git checkout -b <add-your-new-branch-name>
```

For example:
```
git checkout -b add-os-project-name
```
(The name of the branch does not need to have the word *add* in it, but it's a reasonable thing to include because the purpose of this branch is to add an open source project to a list.)

## Make necessary changes and commit those changes

Now open `WOSCA Open Source Projects.md` file in a text editor, add an open source project at the bottom of the table using the format below
```
<tr>
    <td>Project Name</td>
    <td>Description</td>
    <td>Repository</td>
    <td>Stack</td>
    <td>Level of Skill Required</td>
 </tr>
```
Now, save the file.


If you go to the project directory and execute the command `git status`, you'll see there are changes.


Add those changes to the branch you just created using the `git add` command:

```
git add WOSCA Open Source Projects.md
```

Now commit those changes using the `git commit` command:
```
git commit -m "Add <OS-Project> to Contributors list"
```
replacing `<OS-Project>` with open source project name.

## Push changes to GitHub

Push your changes using the command `git push`:
```
git push origin <add-your-branch-name>
```
replacing `<add-your-branch-name>` with the name of the branch you created earlier.

## Submit your changes for review

If you go to your repository on GitHub, you'll see a  `Compare & pull request` button. Click on that button.

Now submit the pull request.

Soon I'll be merging all your changes into the master branch of this project. You will get a notification email once the changes have been merged.
