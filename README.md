# Onboarding

For those new to the lab Github Start here:

## Table of Contents

1. [Navigating the lab Github](#navigating-the-lab-github)
    1. [Key Repositories](#key-repositories)
    1. [Teams and Roles](#teams-and-roles)
        1. [Importance of Teams in Project Management](#importance-of-teams-in-project-management)
        1. [Creating and Managing Teams](#creating-and-managing-teams)
        1. [Setting Repository Access](#setting-repository-access)
        1. [Finding Your Team and Repositories](#finding-your-team-and-repositories)
    1. [Using Git and LFS](#using-git-and-lfs)
        1. [Installing Git](#installing-git)
        1. [Installing Git LFS](#installing-git-lfs)
        1. [Cloning a Repository with Git](#cloning-a-repository-with-git)
        1. [Working with Git LFS](#working-with-git-lfs)
        1. [Pulling Changes](#pulling-changes)
        1. [Creating and Switching Branches](#creating-and-switching-branches)
    1. [Setting Up A New Project](#setting-up-a-new-project)
        1. [Creating a New Repository from the `unity-template`](#option-1-creating-a-new-repository-from-the-unity-template)
        1. [Creating a New Repository from Scratch](#option-2-creating-a-new-repository-from-scratch)
    1. [Repositories](#current-repositories)
1. [Recordings](#recordings)
    1. [Movement in Unity](#movement-in-unity)
    1. [Avatars in Unity](#avatars-in-unity)
    1. [Movement IK (Inverse Kinematics) in Unity](#movement-ik-inverse-kinematics-in-unity)
    1. [Using Headsets with Unity](#using-headsets-with-unity)
    1. [Blender to Unity Workflow](#blender-to-unity-workflow)

(Here, you can continue with the detailed sections as previously written...)


## Navigating the lab Github

In the Virtual Embodiment Lab GitHub, you'll find various repositories to help you get started with Unity and our projects.

### Key Repositories

---

- **[Unity Tutorial](https://github.com/virtual-embodiment-lab/unity-tutorial):** This repository contains tutorials and guides for getting up to speed with Unity, especially tailored for our lab's work.
- **[Unity Template](https://github.com/virtual-embodiment-lab/unity-template):** Use this as a starting point for new projects. It includes predefined settings and assets to streamline your workflow.

### Teams and Roles

---

In the Virtual Embodiment Lab, we utilize GitHub Teams to manage and organize roles within our projects. This approach allows us to assign specific teams to relevant repositories, ensuring that every team member has access to the resources they need for their specific tasks.

#### Importance of Teams in Project Management

- **Structured Collaboration:** Teams enable structured collaboration, where members can work together on projects while maintaining organization and clarity.
- **Role-Specific Access:** Different roles within a team may require different levels of access. For example, project leaders typically need full access to repositories, including administrative rights, whereas other team members might only need read or write access, depending on their responsibilities.

#### Creating and Managing Teams

- **Creating a New Team:**
    1. Go to the [GitHub](https://github.com/virtual-embodiment-lab) page.
    1. Click on "Teams" in the organization's dashboard.
    1. Select "New team" and fill in the details such as team name, description, and repository access levels.
- **Adding Members to a Team:**
    1. Navigate to the team you wish to add members to.
    1. Select "Members" and then "Add a member."
    1. Enter the GitHub username of the individual you want to add and set their role within the team.

#### Setting Repository Access

- **Assign Repositories to Teams:** Each team should be assigned specific repositories relevant to their project. This is done by navigating to the repository settings and adding the team under the "Collaborators & teams" section.
- **Access Levels:**
  - **Read:** Suitable for team members who need to view and clone the repository but do not contribute code.
  - **Write:** For team members actively contributing to the repository, allowing them to push changes.
  - **Admin:** Reserved for project leaders and managers, providing full access to the repository, including settings and access control.

#### Finding Your Team and Repositories

To find out which team you're in and access the repositories assigned to your team:

1. Go to the [GitHub](https://github.com/virtual-embodiment-lab) page.
1. Click on "Teams" in the dashboard.
1. Locate and select your team to view its details, including associated repositories.

By efficiently managing teams and roles, we ensure that every member of the Virtual Embodiment Lab has the right tools and access for their contributions.

### Using Git and LFS

---

Git is a distributed version control system that is essential for managing our project's codebase think of it as Google Drive for code. For handling larger files, such as multimedia assets and datasets, we use Git Large File Storage (LFS). This tool replaces large files in the repository with text pointers and stores the file contents on a remote server. Here's a guide on installing and using Git and Git LFS.

#### Installing Git

1. **Download Git:**
   - Visit the [official Git website](https://git-scm.com/downloads) and download the appropriate version for your operating system.
2. **Install Git:**
   - Run the downloaded installer and follow the on-screen instructions to complete the installation process.
3. **Verify Installation:**
   - Open a terminal (Command Prompt or Git Bash on Windows, Terminal on macOS and Linux) and type `git --version`. This command should return the installed version of Git, confirming successful installation.

#### Installing Git LFS

1. **Download Git LFS:**
   - Visit the [Git LFS website](https://git-lfs.github.com/) and download the installer for your operating system.
2. **Install Git LFS:**
   - Run the installer and follow the setup instructions.
3. **Initialize Git LFS:**
   - Open a terminal and run `git lfs install`. This command sets up Git LFS.

#### Cloning a Repository with Git

1. **Find the Repository URL:**
   - Navigate to the GitHub repository page and click on the 'Code' button to find the repository URL.
2. **Clone the Repository:**
   - Open a terminal and type `git clone <repository-url>`, replacing `<repository-url>` with the actual URL of the repository.
   - This command clones the repository to your local machine.

#### Working with Git LFS

1. **Track Large Files:**
   - To track large files with Git LFS, use the command `git lfs track "<file-type>"`, replacing `<file-type>` with the type of files you want to track (e.g., `*.psd` for Photoshop files).
   - This command should be run in the root directory of the Git repository.
2. **Commit and Push:**
   - After adding or updating files, commit them using `git commit` and push them to the remote repository using `git push`.
   - Git LFS automatically handles the large files tracked by it.

#### Pulling Changes

- To update your local repository with the latest changes from the remote repository, use `git pull`.

#### Creating and Switching Branches

- To create a new branch, use `git branch <branch-name>`.
- To switch to a different branch, use `git checkout <branch-name>`.

This comprehensive guide should help you effectively use Git and Git LFS for managing and contributing to projects in our lab. Remember to regularly commit your changes and stay updated with the latest changes from other team members.

### Setting Up A New Project

---

When starting a new project within our GitHub organization, you have the option to create a new repository from scratch or use the `unity-template` repository as a basis. Here’s how to do both:

#### Option 1: Creating a New Repository from the `unity-template`

1. **Go to the `unity-template` Repository:**
   - Navigate to the `unity-template` repository within our GitHub organization.

2. **Generate a New Repository from the Template:**
   - Click on the "Use this template" button, usually located near the top of the repository page.
   - You'll be prompted to enter the new repository details:
     - **Owner:** Ensure you select our organization.
     - **Repository name:** Enter a name for your new project.
     - **Description:** Optionally, provide a brief description of the project.
     - Decide if the repository should be public or private.
   - Click "Create repository from template" to generate your new project repository.

3. **Clone the New Repository:**
   - Once your repository is created, clone it to your local machine using `git clone <repository-url>`, where `<repository-url>` is the URL of your new repository.

4. **Personalize Your New Project:**
   - Rename any files, update project settings, and modify the project to suit your specific requirements.

#### Option 2: Creating a New Repository from Scratch

1. **Create a New Repository:**
   - Go to the main page of our GitHub organization.
   - Click the "New" button to create a new repository.
   - Fill in the repository name, description, and decide whether it should be public or private.
   - Optionally, initialize the repository with a README, .gitignore, and license.

2. **Clone the Repository:**
   - After creating the new repository, clone it to your local machine using `git clone <repository-url>`.

3. **Set Up Your Project:**
   - Set up your project environment locally by creating new files and directories as needed.

4. **Push Initial Changes:**
   - Use `git add .` to stage your changes and `git commit -m "Initial commit"` to commit them.
   - Push these changes back to the remote repository using `git push -u origin main`.

Regardless of the option you choose, ensure to regularly commit your changes to the repository and keep it updated. This practice is essential for collaboration and maintaining a clear history of your project's development.

### Current Repositories

---

- [Teamwork](https://github.com/virtual-embodiment-lab/teamwork): The inflection points project.
- [Mazeworld](https://github.com/virtual-embodiment-lab/mazeworld_deprecated): The old mazeworld project that was made at Iowa State.
- [PTSD](https://github.com/virtual-embodiment-lab/ptsd): The collaboration with Weill creating a VR exposure module for PTSD.
- [TSI_Framework](https://github.com/virtual-embodiment-lab/tsi-framework_deprecated): Originally this project was a monorepo for everything related to the TSI framework. It has since been deprecated and split into multiple repositories.
- [NVC](https://github.com/virtual-embodiment-lab/nvc): Collaboartion with Dr. Shiri Azenkot's lab to create a VR experience for people with visual impairments.
- [VELLib](https://github.com/virtual-embodiment-lab/vellib): A library of scripts and assets that we use across projects.
- [Out Of Body](https://github.com/virtual-embodiment-lab/out-of-body): The out of body project.

## Recordings

During the Fall 2023 semester, I worked with a group of students and recorded some sessions where we went over some basic concepts in Unity that are helpfull for work in the lab. Here are links to the recordings of these sessions.

### Movement in Unity

**Description:** Learn about the basics of character and object movement in Unity.

**YouTube Video:** [Movement](https://youtu.be/nyihEdlUVJU)

### Avatars in Unity

**Description:** This video covers the creation and customization of avatars in Unity, explaining how to import models.

**YouTube Video:** [Avatars](https://youtu.be/R-eP-TdIhG4)

### Movement IK (Inverse Kinematics) in Unity

**Description:** Understand the concept of Inverse Kinematics and how it is used to create more realistic movements in Unity, especially for character joints and animations.

**YouTube Video:** [Inverse Kinematics](https://youtu.be/LpMwSQruies)

### Using Headsets with Unity

**Description:** Explore the integration of VR headsets with Unity, focusing on setup, configuration, and basic VR interactions.

**YouTube Video:** [Headsets](https://youtu.be/qjS9LUHvYMk)

### Blender to Unity Workflow

**Description:** How to create ormodify models in Blender and import them into Unity.

**YouTube Video:** [Blender](https://youtu.be/lhW3NdT_rh8)
