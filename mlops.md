# MLOps at UKHO 


## plan:

- Brief intro to UKHO & ML at UKHO
- Define MLOps
- Challenges of teams 
  - What does "bad" look like
  - What are the risks of not putting in good practices/standards/pipelines
- What does "good" look like 
  - What are the benefits of adopting good practices 
  - What is the value / benefit 
- What are we doing as an organisation 
  - Git track code, DVC track data and artifacts 
  - End to end pipelines to reproduce model and artifacts 
    - "the disposable model" 
    - environment management (poetry) 
    - cloud compute spin up with cml
  - Automated testing, linting, formatting standards
  - GitFlow + DVC 
  - Automated deployment pipelines 
  - Data management
    - raw data immutable 
    - discoverable, accessible data (S3) 
    - data categorisation/ descriptive statistics
  - Model evaluation 
    - cml continuous evaluation 
    - Pull requests with results 
    - MLFlow [?]
    - Model cards 
  - Monitoring
    - Inspecting performance post deployment 









At UKHO, we work on a vast array of data science problems, many of which requiring highly complex and experimental machine learning solutions. 

Over time as we mature as an organisation, we're constantly exploring new ways to strike the balance between rapid experimental progress and robust, repeatable, production-ready code.  

This blog intends to outline what MLOps is to UKHO, what we're doing and our vision for the future. 

## What is MLOps? 

It's widely touted that [approximately 90% of machine learning POCs never make it to production](https://venturebeat.com/2019/07/19/why-do-87-of-data-science-projects-never-make-it-into-production/), so it's no surprise that organisations are increasingly focussing their efforts on _MLOps_ and UKHO is no exception.

MLOps is a nascent field and as such, there are many different definitions of MLOps and how it differs from dev ops, ML engineering, software engineering, data engineering and data science. The way we see it, MLOps is a mixture of best practices, procedures, and governance that serve to build trust, reproducibility and continuous rapid improvement to machine learning models **in production**. But it’s also about fostering a culture, a way of thinking among a team of data scientists, to always be thinking about value, deployment, and to always strike a balance between short term[?] progress and technical debt. 

[info] define technical debt?

MLOps differs from traditional software engineering dev ops because at a basic level, dev ops in software engineering is about how best to manage code, whereas in machine learning projects, we need to manage both code _and_ data. This is an obvious but important difference, which brings about a number of novel challenges not addressed by the traditional tried and tested dev ops tools and techniques of the software engineering world.

And while the number of tools is ever increasing [insert stat about increase in MLOps papers/ references/ blogs], what is considered "best practice" still varies greatly from organisation to organisation.  

## Challenges of data science teams 


...In part due to adopting poor MLOps practices



What does it lead to?



Unmaintainable models

Slow ability to react 

Outdated models

Low trust in ability to tweak without breaking 

Low trust in model itself



What does good MLOps allow us to do? 



What are we doing at UKHO



What impact have we seen in the team



How are we looking to improve in future 





Resources: 
(curate this list before publishing) 
https://www.accenture.com/us-en/blogs/software-engineering-blog/devops-for-ai
https://dev.to/drelleobrien/video-mlops-tutorial-intro-to-continuous-integration-for-ml-479b
https://github.blog/2020-06-17-using-github-actions-for-mlops-data-science/
https://mlops.githubapp.com/blog.html
https://venturebeat.com/2019/07/19/why-do-87-of-data-science-projects-never-make-it-into-production/
https://towardsdatascience.com/why-90-percent-of-all-machine-learning-models-never-make-it-into-production-ce7e250d5a4a#:~:text=As%20VentureBeat%20reports%2C%20around%2090,something%20useful%20for%20the%20company.
https://martinfowler.com/articles/cd4ml.html
