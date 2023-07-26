---
title: Information for Session Leaders
description: Information for Session Leaders at Biodiversity Genomics Academy 2023
---

> Find all our [planned and proposed sessions here](../sessions)

## Next Steps

### Stage 1

1. Choose your time slot between 1st and 30th September
2. Confirm your session title

I will send you the link to a google sheet where all current sessions are listed (more will be added). Please copy and paste your session to your preferred slot as long as you leave an hour between sessions.

### Stage 2

To be finished by 25th August (ideally). I will send reminders, but please [email me](mailto:sujai.kumar@sanger.ac.uk) at any time if you have questions/thoughts about any of these :-)

1. Decide format - zoom meeting or webinar
2. Get session materials ready - slides/text/examples
3. Set up GitPod, if needed
4. Choosing a repeat session format (live or recorded)

#### 1. Decide format

- By default we want to have zoom meetings where participants are free to ask questions in an interactive environment.
- However, if we end up with, say, more than 30 registrations, then we will ask you if you want to restrict attendance, or switch to a webinar format where only you will be talking live, but participants can ask questions in real time using a text format (Discord or GitHub Discussions or a combination, to be decided).
- Only registered participants can join live sessions and ask questions.
- I will be on hand to coordinate and assist with all formats. So you don’t have to worry about setting up rooms, monitoring questions or chats etc.

#### 2. Get session materials ready

- For each session, we will have a GitHub repository at github.com/bgacademy23/SESSION which will also show up publicly at BGA23.org/SESSION and you will have full write access to this repo.
- This page will have standard basic info such as Title, Description, Who is it for, What you will be able to do by the end of the session, Session Leader / Affiliation, How to register/connect etc.
- This page will also be the place to put/link your training materials. If you already have a preferred format for sharing session materials (google slides, powerpoint, pdf, website, etc) then that’s absolutely fine and we will simply link out to them.
- However, if you want to use markdown files (one or more) that will automatically get turned into web pages at BGA23.org/SESSION, then I can walk you through that. Or if you’d like to do that but don’t have time to figure out, then I’m happy to upload/transform everything to markdown for you.

#### 3. Set up GitPod

If your session requires linux command line access. I will help create a .gitpod.yml in the repo, which will allow users to start a server with software already installed and example files ready to go

For example, for BlobToolKit, I created a [.gitpod.yml](https://github.com/bgacademy23/blobtoolkit/blob/main/.gitpod.yml){:target="_blank"} file for installing the dependencies (conda) and pip installing the code, and also added code for starting the docker containers for the API and viewer, which is also nice for end users as they can see what they need to do on their own desktops/HPC server accounts.

To try it out:

- Click on [https://gitpod.io/#https://github.com/bgacademy23/blobtoolkit](https://gitpod.io/#https://github.com/bgacademy23/blobtoolkit){:target="_blank"}
- It will ask you to sign in using GitHub, and for permission to create a gitpod account using your github credentials (this is safe, it asks for read-only access to your GitHub public profile)
- Then it will ask you to launch a workspace (defaults are fine)
- The workspace should take less than a minute to start and will give you a command prompt, where you can run the `blobtools` command to see that everything is installed.

The longest time in any hands-on bioinformatics training/demo session is often installing software, or even getting people to ssh into custom servers which takes some set up - and is not as useful to the end users because it may not reflect their lack of root access on an HPC/workstation set up. The advantage with gitpod is that people can start the session right away in a browser, AND they can see all the steps that were used to set up the machine. I try to do everything in user space without requiring root access (though of course gitpod machines allow you to be root), so that participants can copy the instructions for installing software on a cluster

I will be on hand to create a .gitpod.yml for your session, which you are obviously free to use in all future training materials as well.

#### 4. Repeat session

- As BGA23 has a global audience, each session will be repeated at least once to make it accessible to other time zones. We would love for you to do a second live session in a complementary time zone but we realise that that’s a big ask. If you can’t do a second live session, we would like for you to specify a day that you/your team are available to take part in asynchronous text discussions (on discord/ GitHub Discussions) with repeat session participants who will have already viewed a recording of your first session.
- You don’t need to specify live/recorded, or the day/time of your repeat session right away but please keep this in mind when submitting your preference for the main live session.
- Just to clarify - we typically expect all session materials/video recordings to be fully public, in the FAIR / sharing spirit of the Earth Biogenome Project. But if this is a problem for any reason, please let me know and we'll think of a workaround.

---

## Background

### Why are we doing this?
The [Earth Biogenome Project](https://earthbiogenome.org){:target="_blank"} aims to sequence ~2M species worldwide in the next decade. The bioinformatics tools and approaches for generating (and then analysing) high quality reference genomes are rapidly evolving and improving. We want a growing community of genomics researchers who will use the best practices in the field.

### Why us?
The [Biodiversity Genomics online conference](https://events.venue-av.com/e/BG23_registration){:target="_blank"} has been fully free, open, and worldwide for three years now from 2020 to 2022. [BG22](https://drive.google.com/file/d/1ScfLz-idIV-Wx_JzzoWdd1hWFywlyim0/view){:target="_blank"} was attended by over 2000 people worldwide,
 
**Biodiversity Genomics Academy 2023** is a new, free online training event in conjunction with BG23, hosted by the Wellcome Sanger Institute in collaboration with other EBP partners like the Darwin Tree of Life, Vertebrate Genomes Project, European Reference Genome Atlas, etc.

We will have a dedicated coordinator ([Sujai Kumar](mailto:sujai.kumar@sanger.ac.uk)) who will be responsible for organising everything - promotion, participant registration, online resources, free computing workspaces, community forums, etc. You get the benefit of a worldwide audience and to help others use your tools, methods, and resources.

### What will it look like

Each session is either targeted at

- beginners, eg an introduction to a concept, or a demo on how to set up and use your approach/ tool/ resource, or
- advanced users, eg a masterclass for regular users addressing complex and nuanced issues with your approach/ tool/ resource

You can choose your audience (beginners or advanced users) and also request more time if you need it. We will use [Gitpod.io](https://gitpod.io){:target="_blank"} if you need it, for pre-configured software environments with pre-loaded data, so you can keep pre-computed analyses ready in case any steps take very long.
