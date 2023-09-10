---
title: Gitpod
description: How to sign up for Gitpod
---

## What is Gitpod?

Several sessions in BGA23 are using Gitpod to provide hands-on experience of installing and using the tools and resources that underpin the Earth Biogenome Project.

[Gitpod](https://gitpod.io){ : target="_blank" } allows you to launch and enter Virtual Machines from your browser and gives you 50 free hours per calendar month, enough for these sessions.

Apart from providing a virtual machine, the .gitpod.yml file for each session (described at the end) also provides a complete record of how we installed the tools/resources needed for each session. Therefore it is a very useful "live" reference for participants on how to install those tools/resources.

## How do I sign up for Gitpod?

If you have registered for a session or signed up for a waitlist, you will get emailed a link to a google form asking you to confirm participation. If the session uses Gitpod, you will be asked to first sign up for Gitpod using the instructions below. Therefore, you MUST do the following steps before completing this form to make sure you can start a Gitpod workspace.

It will take a few minutes each to set up a GitHub account and to set up a Gitpod account if you don't already have them:

1. Click on [https://gitpod.io/#https://github.com/bgacademy23/test](https://gitpod.io/#https://github.com/bgacademy23/test){ : target="_blank" } in any desktop web browser (**Note: Safari sometimes has problems on a Mac, so use Chrome or Mozilla instead)**

2. It will ask you to sign up with a GitHub account. If you don't have one, please get one at github.com

3. Once you are signed in to gitub.com - click on the gitpod.io link above again. It will try to launch a Gitpod workspace using your GitHub login. You will need to give Gitpod permission to access (only) the email address on your GitHub account. Follow the Gitpod prompts to ensure you are a real human and won't misuse their resources. **Note: When it asks you to connect your LinkedIn, you can skip that - you will still get 50 hours :-)**

4. Gitpod will ask you to select which code editor and which machine size to start. The defaults are fine.

6. Once the Gitpod workspace starts (typically in less than a minute), you will see the following in your desktop web browser: a file browser on your left, a text editor top right, and a linux terminal bottom right.

7. In the terminal bottom right, you will see a printed message inside "!"s. This will only be true for the BGAcademy23/test Gitpod workspace linked to above. If you can see this message, that means you have successfully launched the BGAcademy23/test workspace! 

**After you've done this, please go to [gitpod.io/workspaces](https://gitpod.io/workspaces){ : target="_blank" } to delete any running workspaces (in green) so that you don't use up your 50 hours per month :-)**

## How does Gitpod work?

You don't need to know this next bit, but in case you're interested:

- Each BGA23 session that uses Gitpod has its own Github repository
- A file called .gitpod.yml in each session repository specifies how to configure a Gitpod workspace for that BGA23 session
- To launch a Gitpod workspace, we use a link like `https://gitpod.io/#https://github.com/bgacademy23/MitoHiFi` which instructs Gitpod.io to create a workspace using the `.gitpod.yml` file present in `https://github.com/bgacademy23/MitoHiFi`
- You can launch ANY Github repository in Gitpod, even if it does not have a .gitpod.yml, i.e. you can put your own repository in the URL like this: `https://gitpod.io/#https://github.com/myorganisation/myrepository` . Gitpod also works for Gitlab and Bitbucket repositories
- To learn how to create your own .gitpod.yml files, see the [.gitpod.yml documentation](https://www.gitpod.io/docs/references/gitpod-yml){ : target="_blank" }
