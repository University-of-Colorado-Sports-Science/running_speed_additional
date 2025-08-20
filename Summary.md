# 2025 CU Athletic Department Internship Program
Welcome to the home base for the 2025 CU Athletic Department Sports Science internship program! This GitHub repository will be the center of all the work you will create for your internship projects these next 10 weeks! In order to stay organized, please use appropriate file nesting with legible titles, meaningful file names, clear commit messages, commented code, good variable names, and strong note-taking methodology. Everyone has a unique workflow when it comes to data analysis, so it is at your discretion to choose what works for you when deciding on your organization methods.

## Getting Started

###  Installing Git and RStudio
1. Download and install [Git](https://docs.github.com/en/get-started/git-basics/set-up-git)
2. Download and install [RStudio (1.1.383 or higher)](https://posit.co/download/rstudio-desktop/)

### Create a repository from this template
1. Follow [this](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template) guide to create a repository from this template.
2. In the section where you select the Owner, please set it to `University-of-Colorado-Sports-Science` so that all of these repositories stay within our organization. This will make it easier to collaborate with your team and Sports Science staff.
3. Please name the repository `t[team number]p[project number]-data-analysis-2025`. So if you are Team 1 and this is Project 2, your repo name will be `t1p2-data-analysis-2025`. This format will help keep us all organized and using the correct repositories when collaborating.

### Clone the `t[team number]p[project number]-data-analysis-2025` repository in order to collaborate with your teammates and the CU Sports Science staff
1. On GitHub, navigate to the Code tab of the repository.
2. On the right side of the screen, click `Clone or download`.
3. Click the `Copy to clipboard` icon to the right of the repository URL.
4. Open RStudio on your local environment.
5. Click File, `New Project`, `Version Control`, `Git`.
6. Paste the repository URL and enter TAB to move to the `Project directory` name field.
7. Click `Create Project`.

### Next Steps
Now that you have the repository downloaded, open the R Markdown file entitled `data-analysis-2025.Rmd`. This will be the notebook where you are expected to compile your full data workflow with meaningful comments, accurate variable names, create visualizations, and perform your data analysis. Feel free to create additional R notebooks or R script files to explore the workflows you want to implement without doing work in the main document. The main `data-analysis-2025.Rmd` file has a few included libraries and headings to get you started and show some expected formatting. 

The `general-documents` folder will contain a document entitled `Group Assignments.pdf`. This document will list your group members, analysis questions, and which project (1 or 2) the analysis questions should be answered in. Please answer these **in the order they are given** since each is set up to work with the flow of the internship. In general, the first question will be a bit more concise and easier to answer, while the second will be slightly more in-depth since you will already have a flow with your team.

The `general-documents` folder will also contain 2 resource documents for your use. The first, entitled `Internship Program.pdf` is a general outline of the project timeline, the research topics, the supporting data sets, and a bit of context, including some research papers. Please read this document as early as you can to get your bearings and start analysis. The second, entitled `Data Science Internship Background.pdf` contains some literature background related to Hamstring Injuries and Running. This will be helpful for all research topics besides the Men's Basketball RSI topic. The Men's Basketball RSI topic has a few attached papers in the first document, and Tessa will provide additional context outside of these documents to help you get started.

The `data-sets` folder in the repository is the home for all of the deidentified data sets that will be provided to you from the CU Sports Science Team. You will have to extract these data sets from the compressed folder. Please extract them to a folder entitled `data-sets-uncompressed` within the `data-sets` folder. It is **imperative that you name this folder exactly as it appears in this README** or else the `.gitignore` file will not exclude this directory from your repository and Git will throw errors at you when you try to push your repository updates. The data sets, once uncompressed, will be in Comma Separated Value (`.csv`) format. These data sets are deidentified **by sport** so Athlete 1 in Men's Basketball will be a different person than Athlete 1 in Women's Lacrosse. Please keep this in mind when performing your analysis.

The `notes` folder in the repository will be home to all note-taking documents throughout the project. Feel free to upload PDF (`.pdf`), Word (`.docx`), Plain text (`.txt`), Markdown (`.md`), or any other note document to this folder. Note taking is expected in meetings, researching, and general brainstorming. While not explicitly required, it will be helpful to see your thought processes if you encounter roadblocks, so good and thoughtful note-taking will only benefit you in the long-run.

Feel free to create any other folders within the repository as you see fit. All we ask is that you keep the files we provide to you in their original file folder destinations.

# Weekly Schedule
This is a weekly schedule **per project**. The aim of this internship is to complete 2 projects, both of which will follow this schedule.

For the regularly scheduled check-ins, we will meet twice a week. Our first team meeting will take place on Tuesday, June 3, 2025 at 9:30am. Both teams and Sports Science staff will be a part of this meeting as a sort of orientation type meeting. After that, we will start our biweekly meetings using the following schedule:

- Team 1: Mondays @ 9:30am, Thursdays @ 9:30am
- Team 2: Mondays @ 10:00am, Thursdays @ 10:00am

If your team needs or wants additional meetings, please reach out to us and we are happy to add times throughout the course of the internship!

During these meetings we will address 3 main ideas:
1. Your team's to-do list to complete the project
2. Your team's estimated capacity (the first meeting will address how much capacity you have for the week, the second meeting will address how much capacity your team has left this week).
3. The following questions:
  - What have you done since our last meeting?
  - What do you plan on doing before the next meeting?
  - What obstacles are impeding your work?
  
Your team **should not** set a singular project role for each member. Instead, your team is cross-functional, allowing members to work on anything that the team agrees on. 

Finally, the following schedule is your expected in-office hours for **both** teams:

- Monday: 9:00am - 2:00pm
- Tuesday: 9:00am - 2:00pm
- Wednesday: 9:00am - 2:00pm
- Thursday: 9:00am - 2:00pm

This is a tentative schedule that may be subject to change once addressed in biweekly meetings.

## Week 1: Background and Research
Key Deliverables:
1. Project Roadmap
2. Condensed Literature Review
3. First Peer/Performance Review
  
### Project Roadmap

This project roadmap will be the blueprint for your team in completing your project. Broken down into week-by-week milestones, this will guide not only your team, but Sports Science staff in our bi-weekly meetings and give us a better idea as to where you may encounter issues. This roadmap is not intended to be a concrete final document, but a flexible and fluid document that will change based on project flow, discoveries, and additional requirements provided by key stakeholders. Some suggested additions to get your roadmap started are hypothesis statements, documentation style and modality (i.e. we will be taking notes in x format), timelines, work assignments, and/or intra-team meeting schedules. Please put this file in PDF format in the `./general-documents/week-1-deliverables` folder by EoD Friday of Week 1.

### Condensed Literature Review

Within the `general-documents` folder, there will be a document containing compiled relevant literature on the pertinent topic of this project. Using this literature, please find a few more sources and summarize your findings in a 2-3 page document. 1-2 paragraphs per found source will be sufficient. The main objective of this document is to get you thinking about other variables or influences on your data to guide your analysis. Sports Science staff will also be available throughout this week to help verify the viability of your selected sources as helpful or misleading. Please put this file in PDF format in the `./general-documents/week-1-deliverables` folder by EoD Friday of Week 1.

### Peer/ Performance Review
The `general-documents` folder will contain a performance review document entitled `Week 1 Review.docx`. During our Thursday meeting times, a Sports Science staff member will sit down with you and complete a review of the first week. We will cover team cohesion, any roadblocks moving forward, and plans moving forwards. The objective of this deliverable is to keep you on-track and accountable. Please put this file in PDF format in the `./general-documents/week-1-deliverables` folder by EoD Friday of Week 1.

## Weeks 2 - 4: Data Analysis
Key Deliverables:
1. Daily Meaningful GitHub commits
2. Second Peer/Performance Review

### Daily Meaningful GitHub Commits
After week one, the reigns will be loosened, and your team will begin to dive into data analysis. This is a very open-ended section of the project, as you will be able to transform and use the data as you see fit. It is easy to get lost in the weeds or off-track here, so Daily GitHub Commits will allow Sports Science staff to support you and guide you before things become too off-track. The expectation is to log the steps you take to create a reproducible workflow. A "daily" commit means making a GitHub commit each day that your team is scheduled to be on-campus. For example, if your team is here Monday, Wednesday, and Friday, the only expected commits will fall on Monday, Wednesday, and Friday. If you reach a point where you feel there will not be an opportunity to make a meaningful commit for a day, please reach out to the Sports Science staff and we can address this on a case-by-case basis.

### Peer/ Performance Review
Similar to week one, at the end of Week 4, the `general-documents` folder will contain a performance review document. During our Friday meeting times, a Sports Science staff member will sit down with you and complete a review of the second through fourth weeks. We will cover team cohesion, how well Sports Science staff supported you, a wishlist for next project, and a favorites/ most growth section. The objective of this deliverable is to keep you accountable and set up for the next project. Please put this file in PDF format in the `./general-documents/week-4-deliverables` folder by EoD Friday of Week 4.

## Week 5: Conclusion Presentation
Key Deliverables:
1. Final Presentation
2. Final GitHub Repository

### Final Presentation
In a PowerPoint presentation AND written report, your team will be expected to compile their meaningful visualizations, conclusions, and statistical analysis. Please make sure to cover sampling methods (if used), possible biases (and how to limit them), scalability (i.e. adding variables, application to other sports), and defining the data specifically (center, shape, spread, unusual features). Please provide a clear and actionable set of principle findings for the original stakeholder.

### Final GitHub Repository
By EoD Friday of Week 5, your team will be expected to have committed their final changes to the repository. A Markdown file (README replacement) is expected to be pushed to the repo containing the following:
- Project Contributors and their main responsibilites
- Project overview containing a brief summary of the question answered, methodologies used, and any important links/citations
- Clear and concise step-by-step explanation of code implementation
- Summarized final results
- Clear and concise commented code with Authors, Purpose Statement, Author Dates, and Most Recent Update


## Resources

- [Using GitHub with R and RStudio](https://resources.github.com/github-and-rstudio/)
- [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)
- [Additional Useful R Packages](https://support.posit.co/hc/en-us/articles/201057987-Quick-list-of-useful-R-packages)
- [GitHub Cheat Sheet](./general-documents/git-cheat-sheet-education.pdf)
- [Tidymodels Help Page](https://www.tidymodels.org/)
- [Pull Requests Guide](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)
