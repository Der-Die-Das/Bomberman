# Bomberman 

Planing of the Project is on [Hack'n'Plan](https://app.hacknplan.com/p/94601).  
Some thoughts are written down in the [Workflowy](https://workflowy.com/s/bomberman/o4nDcUpt60HgfnmS).

## Table of Contents
- [Creating Tasks](#creating-tasks)
- [Working on Tasks](#working-on-tasks)
- [Reviewing a Pull Request](#reviewing-a-pull-request)

## Creating Tasks
To read about what a **Task** is in the **Hack'n'Plan** sense checkout their [documentation](https://hacknplan.com/knowledge-base/anatomy-of-a-task/).  

To create a new **Task** in **Hack'n'Plan** go to the **backlog** page, click on the ***Add item*** button and select **Task**.  

### Title
Try to give your new **task** a fitting name. For example:  
```
Player Movement
```
### Board
For the board you first choose ***No board***. Later we can discuss when to work on what **task**.

## Description
In the description you write down what you want to be done in this task. Also describe how you want it to be achieved.

## Tags
Add the correct tag to it.  
```Player``` for stuff regarding the player. Like a new mechanic or a gameplay fix.  
```GameDev``` for stuff regarding the developer. A new developer plugin, or documentation.
### Assigned users
Clear the assigned user (yourself) from the list.  
Which user does what work is discussed later, when we pick up the task.

### Sub Tasks
You will want to add some **sub tasks** to the task to have smaller packets that you can work on.  
To do that select the ***Fields*** Dropdown on the top of the window and enable ***Subtasks***.

### Example

Here you see a example of a **Task**:
![Task Creation](/Documentation/TaskCreation.png)

## Working on Tasks

1. First you assing yourself the new **task** in **Hack'n'Plan** and move it to ***IN PROGRESS***.
![Assign Task](/Documentation/AssignTask.png)

2. Switch to new **Branch**.  
    In console you do it as follows:

    ``` shell
    git checkout feat/PlayerMovement
    ```
    The naming should be like this:  
    ***type of work/name of branch***

    *type of branch* could be:
    - **feat:** if you add a new feature
    - **docs:** if you add some sort of documentation
    - **chore:** if you do some work 
    - **fix:** if you fix something

3. Start working
4. Commit regularly. You commit messages should look similar to the branch naming like this:  
        ***type of work: what did you do***

5. After your first commit create a **pull request** on **GitHub**.  
    1. Go to ***Pull requests*** and click on ***New pull request***
    2. Select your **Branch**
    3. Click ***Create pull request***
    4. Add a **Reviewer**
    5. Add an **Assignee** (you if you're still working on it, the reviewer if you're done)
    6. Complete the **pull request**
        - if you're done, select ***create pull request***
        - if you're still working on it, select ***create draft pull request***
   
    ![Pull Request](/Documentation/PullRequest.png)


## Reviewing a Pull Request