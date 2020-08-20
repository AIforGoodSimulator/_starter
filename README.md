# _starter
DB New starter pack and project overview
* More information is available from https://www.notion.so/aiforgoodsimulator/

# Hack from home AI for Good Simulator - Starter Pack
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

\* Scope of work subject to change depending on requirements

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
![Architecture](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/fc7e06a4-f0b4-4651-a6af-070b390cc31d/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5%2F20200820%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20200820T183507Z&X-Amz-Expires=86400&X-Amz-Signature=71e40dd20dc5a45c62af8e1ea5bbde3e0eac67d812cf5d6059013a024b55aed8&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22)

# Model server
Purpose
* A pluggable model layer and standardised parameter handling
* A centralised place to store and run various models based on specified algorithms
* An application that exposes a standard model API via REST microservices

Design
* Top level packages:
  * models -COVID-19 models and model registry
  * params–interface to parameter storage and retrieval
  * runner -console runner for single (one-off) or multiple profiles (batch)
  * webapp-web application runner (with shared state and cache storage) and viewer (configand reporting pages)
* Details in Readme.MD from GitHub repo
* To try: http://ai4good-sim2.azurewebsites.net/sim/run_model

Challenge
* The Model Server has been developed by DB volunteers, jointly with the AI For Good community, to run any supported model with flexibly defined parameter configuration, and render predictions and visualisations on a web application. The Model Server approach seeks to create a pluggable model layer and standardised parameter handling, whilst rendering interactive visualisations and reports via a web application.
* One of the key challenges is to make more models available and to extend the flexibility, accuracy and speed. In taking a model in a language other than Python, we are faced with challenges as to how to integrate with Model Server. 

Reusable platform
* Approaches include:
  * re-write (and re-factor) the model in Python. This requires SME access to understand the model and conversancy with packages required to re-code. The re-written model must respect the parameter and run interfaces and be re-factored to attain required separation
  * separate algorithms from parameters (e.g. SEIR) and input data (e.g. camp data) such that new or updated models can be introduced with minimal changes from the model server
  * create a binding layer whereby model activation and parameterisation can be controlled from Python via an adapter layer
  * potentially extend model server to non-COVID-19 use cases in future
* These approaches are of course not mutually exclusive!

# Team structure*
AI for Good
* The AI For Good simulatorinitiative is organised into a number of areas:
  * Product(co-lead with DB)
  * Model R&D(with academia)
  * Partnership & outreach(NGOs)
  * Field innovation(survey distribution on-site, desktop research)
* DB is going to co-lead the product development with AI for Good
* While the design, engineering and delivery the simulator are recognised as “Product Team” concerns, DB assistance in other areas is also welcome and encouraged. 

Product team
* Project lead
  * John Barclay (CRO, DB)
  * Antoinette Lynch (S&IN, DB) (Consulting)
  * Alice Piterova(MD, AIforGood) (Consulting)
* Project management
  * Peter Hung (S&IN, DB)
  * Sam Meeson-Frizelle (Product Manager, AIforGood)
  * Billy Zhao (CTO, AI4Good) (Consulting)
  * Fabian Rugamer (Microsoftliaison representative)
* Communications
  * Mary Yucedel(Comms& marketing)
  * Fredrika Otterstrom (Communities of Practice)

Technical development
* AI / machine learning model
  * Agent-based model
  * Compartment model
  * Network model
  * Research & Development
* Backend
  * Architecture
  * Cloud & infra
  * Database
* Frontend
  * Web & vis
  * Design & UI/UX
* QA
  * QA front / back / mobile
* Agile
  * Scrum master

\* Team structure subject to change depending on requirements
