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
An *analysis project* would seek data to answer this question
directly.
However, you choose not to actually answer the question
yourself but rather to build
a tool to help
others to answer the question
(e.g., better organize the Pronto data for analysis).
Still another possibility is that you will build a system that teaches
others the skills needed to do analysis
(e.g., a system that teaches about logistics for businesses in the
sharing economy).

Projects may be of many types:
- Analysis projects answer one or more science questions.
- Tool projects create software or data resources intended for use by others.
- Instructional projects create an environment intended to teach specific material.
Other types of projects are possible as well.

## Project Workflow

### Step 1: Pick Your Data
You should have two data sets so that you can demonstrate an ability
to join data with different characteristics (e.g., granularity in time and/or space)
The data must be available immediately, without concerns
about access rights for team members or the instructors.

### Step 2: Define the Problem
Determine the type of project  (e.g., analysis project) and the
questions of interest.

### Step 3: Write the Functional Specification
The functional specification details:
- Who are the users and what do they know (e.g., business analyst)
- What information users want from the system (e.g., where to put bicycles)
- Use cases - how users interact with the system to get the 
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
- README.md file that gives an overview of the project
- LICENSE file
- setup.py file that initializes the project after it has been cloned
- doc folder that contains documentation (including the functional specifical
and the design specification)
- python package folder (with the same name as the repository)
that is structured as one or more python modules 
(e.g., with __init__.py files) and test files that begin with "test_".
- examples folder that contains examples of using the packages

## Presentations
Projec teams 
will present their projects, either as a poster or a 25 presentation.
The presentation should include:
problem description and motivation,
data used,
use cases,
design,
demonstration (either live or in screen shots).

## Grading Rubric
Projects will be evaluated based on the following criteria:
- Organized as described in the section on project structure
- Quality of the documentation (especially the functional
specification and design specification)
- Code quality, especially consistent coding standard
- Test coverage
- Quality of the example of using the package (in the examples
folder of the project repository)
- Completeness of the setup.py script
