---
title: Information for Session Leaders
description: Information for Session Leaders at Biodiversity Genomics Academy 2023
---

> Find all our [planned and proposed sessions here](sessions.md)

This page has been updated on 2023-09-10. Older information can be found [here](session-leaders-20230909.md) 

## Week 1 Update

- The first BGA23 session (Mon 4 Sep 08:00 UTC) on BlobToolKit ran as expected, but 5 min after it ended, the datacentre that hosted [BlobToolKit](https://blobtoolkit.genomehubs.org){ : target="_blank" } and [GoaT](https://goat.genomehubs.org){ : target="_blank" } went down for 3 days. So we had to postpone the Mon and Wed sessions for these two resources till later in the month
- The first two Gitpod sessions (Fri 8 Sep) on [Treeval](https://BGA23.org/treeval-curation) and [MitoHiFi](https://BGA23.org/MitoHiFi) went very well, with all participants able to launch and follow along with the Gitpod based examples and exercises.
- We now have a total of 2217 initial bookings, 1650 waitlist signups, and over half of the initial sign ups (1161) have confirmed in a second form that they will participate - this is great news!

## Reminder - Add your session materials to Github

- Please add your session materials to your Github session repository at [github.com/bgacademy23](https://github.com/orgs/BGAcademy23/repositories){ : target="_blank" }. The name of your session repo will be the same as the shortname you chose when filling out the session information form, and the same as the link to your session page at [sessions.md]
- If you don't have access, let me know and I'll send another admin invitation to your github username
- Or just send me a link / text and I'll add that to your page
- You don't have to use the Github repo to host your session materials (slides/tutorials), but I would like the starting point to be BGA23.org/session-repo, and have that link to wherever you want to store the materials (eg google slides, a PDF, another github repo, github wiki, etc)
- If you want to use the BGAcademy23 github repo to store your materials, add it under the docs/ subfolder using markdown files.

??? info "**Default Github repo structure**"

    ```
    session-repo/
    ├── .github
    │   └── workflows
    │       └── build-mkdocs.yml
    ├── .gitpod.yml
    ├── LICENSE
    ├── README.md
    ├── docs
    │   └── README.md
    └── mkdocs.yml
    ```

??? info "**How to edit your BGA23.org/session-repo**"

    Note: Replace `session-repo` below with your session's repository name (this is the shortname you chose in the session info form)

    - Edit docs/README.md (markdown format) to change BGA23.org/session-repo
    - There is a shortcut on the top right of BGA23.org/session-repo that takes you straight to the file on GitHub if you want to edit it there
    - If you make any changes to docs/README.md - you should also make them to README.md (you don’t have to, but the main README.md is what shows up when people visit GitHub.com/bgacademy23/session-repo )
    - When you make any change to the repo and commit/push it back, it starts a GitHub action (in .github/workflows/build-mkdocs.yml)
    - The action takes about 1 minute to run and you will get an email notification when finished. After it finishes, the page at BGA23.org/session-repo will be updated.
    - If BGA23.org/session-repo doesn’t look like it’s changed, do a hard refresh in the browser (Ctrl R or Cmd R on some systems)
    - If you have docker locally, you can test changes locally before pushing by running the following, and then visiting localhost:8000 in the browser:
    ```
    git clone https://github.com/bgacademy23/session-repo
    cd session-repo
    docker run --rm -it -p 8000:8000 -v ${PWD}:/docs squidfunk/mkdocs-material
    ```
    - If you want to add any more pages, create them inside docs/ , eg
    ```
    docs/part1.md
    docs/links.md
    ```
    - Navigation for additional pages:
        - In docs/README.md or other markdown pages, if you add a link to [part1.md] or [links.md] or [README.md] it will build the links correctly on the final web pages
        - In mkdocs.yml  add extra top level links (and nested links under the “nav” section, eg
    ```
    nav:
        - Home: README.md
        - Part 1: part1.md
        - Part 2:
            - Nested Link: links.md
        - BGA23: https://bga23.org
    ```

??? info "**If your session needs Gitpod**"

    - If your session needs GitPod, edit the .gitpod.yml file in the root directory of your github repo, otherwise you can safely ignore it :-)
    - This is a minimal GitPod configuration that installs mamba/conda
    - To use it, paste this URL into your browser: https://gitpod.io/#https://github.com/bgacademy23/session-page (replace `session-page` with your github repo name). It will ask you to sign in with GitHub - this is safe
    - https://www.gitpod.io/docs/references/gitpod-yml has the syntax, but I can help you set yours up. We’ve so far managed to set up complex dependencies, docker containers, jbrowse webservers, and even a VNC session if you want participants to launch an X-windows application like pretextview.
    - You can see two examples at https://BGA23.org/treeval-curation/Tutorial and https://BGA23.org/MitoHiFi - both of which have links to launch Gitpod workspaces, and instructions for what to do once you start the workspace.
    - Each participant gets 500 credits per calendar month for free when they log in with their GitHub account (enough for 50 hours of a standard machine - 4 Cores/8GB RAM/30 GB HDD, or 25 hours of a large machine 8 cores/16 GB RAM/50 GB HDD)
    - Participants don’t share gitpod resources with other participants - so each participant WILL get 4 cores, 8GB RAM, 30 GB HDD to themselves when they launch a standard workspace

## Session Leaders are welcome to join all sessions

As a session leader, you're very welcome to join any of the sessions! The zoom link and add-to-calendar link for each session are in the Spreadsheet for Session Leaders that I've already emailed you a link to

You're also welcome to send the Discord link and Zoom link to any colleagues who you want to invite to your session.

## Participant workflow

In case you're wondering, here's what the booking experience is like for a participant:

- Visit BGA23.org/sessions which redirects them to a tickettailor.com session page ([full list here](https://buytickets.at/bga23){ : target="_blank" })
- Book an empty slot (if available). This counts as an initial booking. Else they put their email on a waitlist for that session
- All initial bookings receive an invitation to confirm their booking by the deadline of the Thursday of the week before that session. This confirmation is a prefilled google form. If the session uses Gitpod, the form requires them to sign up for a Gitpod account and make sure it works before they can submit the form (you can try it out [here](https://docs.google.com/forms/d/e/1FAIpQLSeSoJ0mNImSBvg1mmtnaluQ_iRzCTnGJZV_GdZHxjIlFM9EPg/viewform?usp=pp_url&entry.873730893=Sujai+Kumar&entry.2000806590=sujaikumar@gmail.com&entry.115230335=Fri+15+Sep,+09:00+-+Genome+profiling+using+GenomeScope+-+https://BGA23.org/genomescope+-+GITPOD&entry.1835238055=Yes+I+want+to+attend+the+session){ : target="_blank" })
- After Thursday, if all spaces for a session are not confirmed, then I invite all the waitlisted participants to also fill out the form and confirm participation on a first come, first served basis.
- Once they confirm participation, I send out the zoom link for that session to confirmed participants.
- We did it in this two-stage way because a lot of people sign up for a session as it is free, but then realise they can't come, or are not interested based on the detailed description and prerequisites
- This also gives us a chance to remind the participants to actually turn up for the sessions :-)
- For sessions where the leaders have said they don't want to limit attendance, I send session details to EVERYone on the initial booking list and waitlist.