# ml_weather_tutorial
Tutorial material for using machine learning in weather science research


# Hackathon / Tutorial Environment Setup 

In this tutorial we will be using Jupyter Hub on Spice. 
We will be using conda environments for running the data science and machine learning libraries required for this tutorial. 
It would be best if everyone can try setting up their environment before the start of the tutorial to help things to run smoothly.  

## Setup Steps  

Follow these steps to prepare your compute environment to run the tutorial notebooks.

### 1. Clone this repository onto your VDI

Open a linux terminal (for Met Office staff this can be on a VDI, Spice or similar)

Navigate to the folder you wish to store this tutorial in, and clone the repiository using:

```bash
$ git clone https://github.com/informatics-lab/ml_weather_tutorial/ 
```

### 2. Build the `conda` environments for this tutorial


If you have never used `conda` on your VDI before, please follow these instructions to set it up with the required Met Office security precautions:<br>
https://metoffice.sharepoint.com/sites/TechnologyCommsSite/SitePages/Tooling/Artifactory/Authenticating-Conda-with-Artifactory.aspx 

You can check whether `conda` is working correctly by running the following command, which should list all available `conda` environments on your system:
```bash
$ conda env list
```

You can then build the `conda` environments needed for these tutorials using the following commands (these can take a few minutes to complete):
```bash
$ cd ml_weather_tutorial
$ conda env create --file environments/req_sklearn_spice_lock.yml
$ conda env create --file environments/req_tensorflow_spice_lock.yml
```

### 3. JupyterHub on SPICE

For these tutorials we will be using JupyterHub on SPICE. This gives us access to more compute resources on SPUCE than using the VDI, and a convenient Jupyter interface to run the tutorial notebooks.

Start your own JupyterHub session on SPICE by going to https://jupyterhub.metoffice.gov.uk/. We recommend launching it in a web-browser on Windows for a smoother experience, but it will work on your VDI too.

You will need to log in with your **LINUX** username and password, the same used to log into your VDI (**not** your Windows username or email address).

You will then be presented with the usual SPICE option for requesting CPUs, memory and an amount of time. We recommend at least 2 cores, 8 GB of RAM and 300 minutes for this tutorial.

For more information on how to use JupyterHub on SPICE, please watch this 4 minute video:
https://web.microsoftstream.com/video/99527d1c-d4b2-47b7-9477-9adb70485a05  


---
# ML Tutorial & Hackathon Prospectus 
Delivered by the Informatics Lab 


## Introduction 
In 2022, the Informatics Lab was asked to facilitate a machine learning hackathon for a team in the Met Office that was interested in applying ML to their area of research but felt they did not have the skills required to get started and so wanted to follow a pattern to other teams and organisation and have a concentrated team activity focused on ML to kick start things. The Informatics Lab was approached ads the leading data science and machine learning team in the Met Office to facilitate this.  

The success of hackathon, whatever the aims of the hackathon (for example in this case the main outcome is skills development, rather than protype development as it is in other hackathons), depends on the preparation. In the case of these hackathons, a lot of the participants are new to machine learning and so need some training to get up to speed or approach the subject in a more systematic before so they have the skills required to get the most from the hackathon. As a result, a tutorial was developed to be delivered over two half day sessions, with a gap in between to allow for the information to be digested and tried out.  

Another aspect of preparation is to have ideas fleshed out before the day so participants have a clear idea of what they will be doing during and what they want to get out of the time they spend on the hackathon. Part of this is that we have a time at the end of the tutorial to have an ideas generation session to flesh out ideas from day-to-day wok or that might have been stimulated by what was learned in the tutorial.  

This is also a time to decide what will need to be done in slower time between the tutorial and the hackathon itself. In particular, retrieve and organising data may take a long time (mostly waiting for copying and process rather than active involvement), so should be done before the hackathon so as to use the hackathon time most effectively 


## Basic Syllabus 
- Part 1 – Exploring your data 
- Part 2 – Building a machine learning pipeline 
- Part 3 – Algorithm Deep Dive 
- Part 4 – Improving performance 


## Key outcomes 
Participating Team 
- Introduction to machine learning – basic theory and practical examples 
- Opportunity to try out ML knowledge with assistance from lab tutors 
- New ideas for using ML in team research area 
- Understanding of Met Office strategy and best practices around use of machine learning 

Informatics Lab 
- Build connections with other areas of office  
- Build awareness of data science framework  


## Resources required 
From the team 
- Total time commitment for participants in sessions 2.5 days 
  - 2x4 hours tutorial 0.5 day for hackathon prep, 1 day for hackathon 
- Organiser lead  commitment – ~1 day 
- Book a venue (ideally in the Met Office College) 
- Set up MS Teams meetings to enable remote participation 
- Find suitable dates for participants and tutors from Informatics Lab 

From the Informatics Lab 
- Provide training material 
- Provide tutors for tutorials and hackathons 
  - 1 trainer and 2 helpers for group of 20 recommended 
  - 3-5 tutors for hackathon, depending on number of participants and groups (approx 1/group or 1/6 participants) 
- Link to training material: https://github.com/informatics-lab/ml_weather_tutorial/  


## Sessions Breakdown 
Session 1 
- 00h00 Introduction (20 Minutes) 
- 00h20 Notebook 1 – Data Exploration (40 Minutes) 
- 01h00 Practical 1 – Data Exploration (40 Minutes) 
- 01h40 Break (15 Minutes) 
- 01h55 Notebook 2 – ML Pipeline (55 Minutes) 
- 02h50 Practical  2– ML Pipeline (40 Minutes) 
- 03h30 Questions & Ideas Generation (30 Minutes) 

Session 2 
- 00h00 Recap and Intro (10 minutes) 
- 00h10 Notebook 3 – Algorithm Deep Dive (50Minutes) 
- 01h00 Practical 3 – Algorithm Deep Dive (30 Minutes) 
- 01h30 Break (15 Minutes) 
- 01h45 Notebook 4 – Improving Results (45 Minutes) 
- 02h30 Practical 4 – Improving Results (30 Minutes) 
- 03h00 Hackathon Planning & Ideas (30 Minutes) 
- 03h30 Practical Session (30 minutes) 

Hackathon 
- 09h30 Brief intro to each project and plans for the day 
- 10h00-12h30 Split into groups 
  - Decide on priorities 
  - Work on hackathon idea 
- 12h30-13h30 Lunch 
- 13h30 Report on Morning 
  - Progress so far, next steps, blockers 
- 13h45-16h30 – Split into groups 
- 16h30-17h00 – Report back & Close (5 mins per group) 
  - Key Outcomes (plots, demo code, lessons learnt) 
  - Next Steps (how is this idea going to be taken forward?) 
 

 
