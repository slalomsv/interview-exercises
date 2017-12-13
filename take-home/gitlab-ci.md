# Take Home Assignment 1: Docker with GitLab-CI

## Requirements & Setup
- Install [Docker](https://docs.docker.com/engine/installation/)
- Create a free [GitLab account](https://gitlab.com/users/sign_in) or re-use your existing one if applicable.
- Create a [new project](https://gitlab.com/projects/new) and set the visibility level to "Private"
- Create a new branch named "master" and set it as the default branch with protection enabled.
- (The remainder of the instructions specific to GitLab are a part of the exercise and are intended to be learned/discovered by the candidate).


## Objective
**GitLab CI:**
- Build and push a simple Docker image to the GitLab Registry associated with your project.
- The CI job should be automatically triggered on every repository push. 
- The image should be named "slalom" and tagged as follows:
    - When merging to the "master" branch, the tag will be ":latest"
    - When pushing to a non-master branch, the tag will be the first 12 letters of the git commit hash

**Docker:**
- The Docker container should use Python to serve a set of static web pages via port 8000
    - Resource paths "/" and "/index.html" should serve a page which says "Hello, Slalom!" and has a title of "Slalom Consulting".
    - Resource path "/admin.html" should serve a page which contains a timestamp of when the container first came online.
        - The timestamp should be in "YYYY-MM-DD HH:MM:SS" format.
    - The style of these pages does not count towards submission credit, so keep it simple.
    - While you must use Python to serve the content, you do not need to implement a webserver yourself.


## Submission
The final product must be turned in prior to the deadline specified by the interviewer/recruiter. Please ask if this was not shared with you.

You may submit it in via email and package it in one of two ways:
1. (Preferred) A direct link to the repository. You will need to grant explicit access to the project to one of the interviewers' GitLab accounts -- they will provide this if necessary.
2. Zip/tar/compress a local copy of your project as it appears in the repository and attach it to your submission email.  Also include a screenshot of your GitLab Registry page showing you successfully pushed the required images:tags as a result of the CI pipeline.

**Note:** You should include links to any referenced material in your comments or README file. We understand that learning does not exist in a vacuum and Google is a powerful tool -- all we ask is that you cite your sources.


## Tips
- You are encouraged to start early and give yourself adequate time to finish the assignment. Time investment will vary depending on your level of understanding/expertise in the involved technologies, however it is designed such that you can finish this without any prior knowledge of the specific tools used.
- You are encouraged to email questions to the interviewer(s) to solidify your understanding of the objective and clarify any ambiguities you perceive. Please make every attempt to read about relevant topics beforehand and only reach out when you are stuck or something is unclear.  The interviewer reserves the right to answer at their own discretion.
- Treat your interviewer(s) as a client. You should build an understanding of Docker and GitLab CI that extends beyond the bounds of the assignment and be prepared to answer followup questions we may have during or after the assignment window.

## Final Notes
- This exercise is meant to be both a fun learning exercise and a demonstration of your technical problem solving and system architecture abilities.  Please feel free to share your feedback with the interviewer and/or your recruiter once you are finished as we are always looking to improve the experience we provide to candidates.
- Please be respectful of the time and effort put into organizing this exercise by not sharing any details about the problem on Glassdoor or any other forum -- we would prefer all candidates approach this exercise from a level playing field.
- Thank you for your time!
