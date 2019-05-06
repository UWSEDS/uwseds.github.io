---
layout: page
title: Projects
collection: main
---

## Overview
The course project is a "capstone" that pulls together all elements of the course:
data, programming, coding style,
version control, testing, design, and team collaborations.
This is a team effort, often with members drawn from different disciplines.

Projects will address a science or business question of interest.
For example, a business question related to the
bike sharing company Pronto might be "How should bicycles be allocated
among stations?"
An **analysis project** would seek data to answer this question
directly.
However, you may choose not to answer the question
yourself.
Rather, you might do a **tool project** that builds
a tool to help
others to answer the question.
For example, one such tool might be a package that
better organizes
the Pronto data for analysis.
Still another possibility is that you will build a system that teaches
others the skills needed to do analysis, which
we call an
**instructional system project**.
An example here would be
a system that teaches about logistics for businesses in the
sharing economy.
Other types of projects are possible as well.

## Project Workflow

### Step 1: Pick Your Data
You should have two data sets so that you can demonstrate an ability
to join data with different characteristics (e.g., granularity in time and/or space).
The data must be available immediately, without concerns
about access rights for team members or the instructors.

### Step 2: Define the Problem
Determine the type of project  (e.g., analysis project) and the
questions of interest.

### Step 3: Write the Functional Specification
The functional specification details:

* who are the users and what do they know (e.g., business analyst)
* what information users want from the system (e.g., where to put bicycles)
* use cases - how users interact with the system to get the 
information they want

For tool projects, the users are typically programmers, and so the
functional specification describes the programming interface.

### Steps 4 and beyond: Iteratively Develop And Refine the Project
You will organize the project as a set of short-term deliverables.
Typically, you focus first on those parts where you have
the most uncertainty since projects typically fail because
of "unknown unknowns".
For some projects, this will be a data-first focus to make sure that
your data can answer the questions that you pose.
For others, it may be exploring a python package that you hope
will provide key features (e.g., visualizations).

## Project Structure
Projects should have a github repository with the project name.
Top level folders/files within the repository include: 

* README.md file that gives an overview of the project
* LICENSE file
* setup.py file that initializes the project after it has been cloned
* doc folder that contains documentation (including the functional specification,
the design specification, and the final project presentation or poster)
* python package folder (with the same name as the repository)
that is structured as one or more python modules 
(e.g., with __init__.py files) and test files that begin with "test_".
* examples folder that contains examples of using the packages

## Design Documents

You will create two documents describing the design of your project. 
These documents should be in your project ``docs`` folder.
- **Functional Specification**. The document should have the following sections:
  - Background. The problem being addressed.
  - User profile. Who uses the system. What they know about the domain and computing (e.g., can browse the web, can program in Python)
  - Data sources. What data you will use and how it is structured.
  - Use cases. Describing at least two use cases. For each, describe: (a) the objective of the user interaction (e.g., withdraw money from an ATM); and (b) the expected interactions between the user and your system.
  
- **Component Specification**. The document should have sections for.
  - Software components. High level description of the software components such as: *data manager*, which provides a simplified interface to your data and provides application specific features (e.g., querying data subsets); and *visualization manager*, which displays data frames as a plot. Describe at least 3 components specifying: what it does, inputs it requires, and outputs it provides.
  - Interactions to accomplish use cases. Describe how the above software components interact to accomplish at least one of your use cases.
  - Preliminary plan. A list of tasks in priority order.

## Technology Review Presentation
The technology review is about making decisions about the choice of a python library to address a technology need in the project. For example, many projects make use of map visualizations. There are many python libraries that support these visualizations such as Bokeh, Dash, and googlemaps. The libraries have different capbilities, such as what (if any) interactions users can have with the map. You will want to choose a library that: (a) addresses the requirements of your project; (b) is compatible with other elements of your project (e.g., runs on python 3); (c) is relatively easy to use; (d) is computationally efficient for the scale of data you use; and (d) doesn't have software bugs that will impair your use cases.

The technology review is a group presentation. It should be about 15 minutes in length. The presentation should address the following:

- Brief background on the problem you're solving to motivate a technology for which you need a python library (e.g., interactive maps).
- One slide desciption of a use case in which the technology is required.
- One slide that describes at least two python libraries that potentially address your technology requirement.
- For each libarary, show a simple example of using it to implement the use case described above. This means that you will need to install each of the python libraries and attempt to use them.
- One slide side-by-side comparisons of the technologies.

## Project Presentation
Teams 
will present their projects using slides in
15 minute oral presentation.
The presentation should include:

- Background. Describe the problem or area being addressed.
- Data used. What data did you use? How was it obtained? What are its limitations?
- Use cases. How users will interact with your system in a way that addresses the problem area.
- Demo. Demonstrate your software.
- Design. Describe the components and how they interact to accomplish the use cases.
- Project Structure. Show the structure of your github repository.
- Lessons learned and future work.

You should post a PDF of your presentation in the docs folder of your project.

## Grading Rubric
Projects will be evaluated based on the following criteria:

* Organized as described in the section on project structure
* Quality of the documentation (especially the functional
specification and design specification)
* Uses at least two data sources
* Code quality, especially consistent coding standard (e.g., ``pylint``).
* Test coverage
* Quality of the example of using the package (in the examples
folder of the project repository)
* Implements continuous integration (e.g., via travis-CI), and all tests pass.
* Completeness of the setup.py script
* Creativity and technical challenge

## Examples of previous projects
These examples are fantastic, though they may not be perfect. They should be considered examples of what kinds of projects are possible and not necessarily exa mples to be precisely emulated.  The examples below include an analysis project, a visualization project and a reusable data project.

### Spring, 2018
* [Crash Data Analysis Tools](https://github.com/johnash1990/crashDataAnalysisTools) - This set of tools takes several different traffic data sets and merges them as well as providing an easy interface for interacting with the data.

### Spring, 2017
* [First Stop](https://github.com/sliwhu/UWHousingTeam) - First Stop for First-time home buyers; This tool would be most helpful to first-time home buyers to set up expectations, plan budgets and make an informed decision on expenses before they even go through the exhaustive house-hunting process given current real-estate market status.
* [Searching For Success](https://github.com/khyatiparekh/Searching-for-Success) is a template project that can help an amateur investor to visualize search trends on Google for selected company and get probability that the stock price will increase when the quarterly reports will be released for that company.
* [Ax/Wx](https://github.com/rexthompson/axwx) - Ax/Wx is a collision and weather analysis tool that can enhance the WSP collision database with objective observations from nearby personal weather stations. 
* [HomeIn](https://github.com/hanghu/HomeIn) - HomeIn provides a visualization tool for housing data, prices, and crime rates on a multiple-layered map. 
* [How is Uber changing Taxi in New York City?](https://github.com/HWNi/DATA515-Project) Uber is a new riding model which connects drivers and passengers and provides ride-sharing service with a fair rate. This visualization tool enable user to analyze and compare Uber and taxi traffic of neighbors in NYC.
* [AirbnbViz](https://github.com/wangbeiqi199159/AirbnbVizTool) aims to provide more information and insights to guests of Airbnb in Seattle to help them have a deeper understanding of what factors influence the listing price most, which neighborhood has higher/lower listing price and which neighborhood has higher and lower guests' rating via our different interactive visualizations. On the other hand, As hosts of Airbnb, they will have more idaes that how other hosts priced around them relative to dimensions such as amenities and location and what is the average listing prices of different neighborhoods in Seattle.



**ALL INFORMATION MUST BE POSTED TO YOUR REPO BY MIDNIGHT PDT TUESDAY DECEMBER 11, 2018.**
