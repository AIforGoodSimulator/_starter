# _starter
DB New starter pack and project overview
* More information is available from https://www.notion.so/aiforgoodsimulator/

# Hack from home AI for Good Simulator
Starter Pack
Content
* Getting started
  * Executive summary
  * Welcome!
  * What we will do
* Approach
  * Scope of work*
  * Technical environment
  * Conceptual architecture*
  * Model server
* Volunteering-as-a-team
  * Team structure*
  * Team scope*
* What's next
  * To-do
  * Student mentorship
  * Reference links
  * Social media

\* Details subject to change depending on requirements

# Executive summary
Deutsche Bank will help model COVID-19
* Given the unprecedented societal impact of COVID-19, it became clear that crisis modelling of large populations, would be essential for strategies to manage the virus and its transmission
* Our focus on engineering culture and technological innovation, meant that DB could not only offer computational power, but also the expertise behind it, and a sand-box to play-in
* Data insights engaged with the AI/ML Community of Practice and DBIO to explore how the bank could best collaborate with external research groups
* We decided to partner with AI for Good, as they had already established a ‘Simulator’ to model the potential contagion impact of an outbreak of COVID-19 in a refugee camp
* We aspire to provide value to our NGO partner such that refugee camp managers around the world can use the app to reduce and mitigate the COVID-19 outbreak and potentially save lives

# Welcome!
Introduction
* AI For Good is an external organisation focused on harnessing AI for socially, ethically and environmentally positive themes and problems. In particular AI For Good has initiated a volunteer programme called the AI For Good Simulator, which is creating coronavirus modelling, visualisation and reporting solutions for NGOs involved in refugee camps around the world.
* DB volunteers and others are welcome to join, collaborate and contribute. Microsoft have kindly provided a dedicated Azure cloud compute/storage environment, based on DB Hackathon.
* This starter pack will provide you the information you need to start the journey. 

Coronavirus simulator
* The challenge is to model and understand the dynamics and variables or the spread of disease (COVID-19) using data science and mathematical models. In particular there are three models, in varying stages of development and in a number of programming languages, for simulating coronavirus spread and effects in refugee camps, based on configurable camp parameters and inputs.
* The initial ask with respect to the DB volunteers has centred around providing assistance for:
  - Visualisation
  - Web applications
  - Technical and Infrastructure
* While the design, engineering and delivery of such are recognised as “Product Team” concerns, DB assistance in other areas is also welcome and encouraged. 

# What we will do
Actions for DB
* Introduce data quality standards for clean and repeatable model parameterisations and substitutions in the data management layer
* Reduce complexity of source code by using a single language, such as Python
* Focus on widely-used, open source tools & frameworks, such as Python, Plotly-dash, Flask framework and PyCharm
* User Interface (UI) Design

Duration
* August –October 2020, in 2-week sprints
Abstract User Interface (AUI) meta-models that facilitate the different levels of abstraction between the underlying models

# Scope of work
Categories
* Machine learning model engineering
  * Model implementation
  * Model refactoring
  * Translation to Python
  * Model server upgrade
* Backend
  * Azure cloud instance setup and admin
  * AKS DevOps setup
  * Database setup and admin
  * Architecture design
* Frontend
  * Interactive visualisation in plotly.dash / flask
  * Web app foundations (e.g. access control, menu)
  * Design and UI/UX review and analysis
* QA
  * Front / back / mobile
  * CI / CD
* Agile
  * Team of scrum masters
  * Agile ceremonies
* Communications
  * Marketing and communications
  * Communities of Practice (CoP)
* Product management
  * Liaising with AI for Good team
  * Feedback from end-users
  * High-level planning
  * Student mentorship

/* Scope of work subject to change depending on requirements

# Technical environment
* Languages
  * Python (foundational language for models, model server and core infrastructure)
  * Netlogo(Agent based simulation model -note that the predominant python equivalent is mesa)
  * R (used for the Network Model)
* Data layer
  * simple JSON parameter document model
  * MongoDB (Community version)
  * Others : python, pandas, sklearn
* Cloud, compute and storage
  * Microsoft Azure cloud
  * Azure Kubernetes Service (AKS)
  * Azure cloud shell/CLI
  * Azure data science Virtual Machines (VMs)
* Visualisation
  * Plotly-Dash / Flask
  * pandas, Seaborn, Flask

# Conceptual architectural diagram
https://www.notion.so/aiforgoodsimulator/Backend
