# Research Software

Includes source-code files, algorithms, scripts, computational workflows and executables that were created during or for the reasearch the research process.

# Challenges of Research Software Engineering

- Short-lived funding and project longevity
- Lack of software engineering practices
- Rapidly evolving and changing environments
- Reproducibility and open science
- Recognition and career progression
- Interdisciplinary collaboration

# Commit messages

*Blueprint*

```
<type>[optional scope]: <description>
```

*types*

- docs: new documentation
- feat: new feature
- fix: new bug fix
- perf: performance imrovements
- refactor: architecture changes
- style: style changes
- test: new test

*description*

- In imperative and present tense exp.: "change" or "add"
- lowercase first letter
- no sentence punctuation

# Branch based workflow

Developers create seperate branches for each new feature or bug fix. They enable isolation and parallel development and keep the main branch clean.

# Merge conflicts

*Definition*

Occur when two branches made different changes to the same part of the code and are merged. Git cannot automatically decide which version to keep, so it marks the conflicting area for yout to resolve.

*How to resolve*

1. Open file
2. Keep the lines you want and remove others
3. Remove conflict markers
4. Save file
5. git add & commit

# Fork based workflow

Developers duplicate a repository to have a seperate development line.Mostly used for personal development seperated from main development.

# Python style (PEP8)

The official styleguid for python code is PEP8. It fosters readability and convention.

*Spacing*

- Always indent code blocks using 4 spaces, and use spaces instead of tabs.
- Do not put spaces inside parentheses.
- Always use spaces around comparisons like `>` and `<=`.
- Put two blank lines between each function definition.
- Add an empty line at the end of the script.

*Naming*

- Use `ALL_CAPS_WITH_UNDERSCORES` for global variables.
- Use `lower_case_with_underscores` for the names of functions and variables.
- Avoid abbreviations in function and variable names.
- Use short names for short-lived local variables and longer names for things with wider scope.
- Do not comment and uncomment sections of code to change behavior.

*Docstrings*

- Add a file docstring
- Add docstrings for each function

# Jupyter Notebooks

Are interactive computing environments. They combine live code with visualisations and explanatory text. It can be a interactive and exploratory approach for data analysis and workflows. It contains of cells which a type of content. The files are in a JSON-based format.

*Advantages over plain Python*

- Interactive
- Direct visualisations
- Direct documentation
- Exploratory
- Collaboratory through multilingual support 

*Disadvantages over plain Python*

- Complexity
- Limited portability
- Version control is more difficult

# Project metadata

- CITATION.md
- CONDUCT.md
- CONTRIBUTING.md
- LICENSE.md
- README.md

# README.md structure

1. Titel
2. Description
3. Installation
4. Usage
5. License
6. Citation
7. Contact

# Licenses

*Permissive License*

Others can use, modify distribute work under conditions. Allows for combination of licenses and has few restrictions.

Examples: MIT, Apache 2.0, BSD

*Copyleft License*

Derivative works/modifications of work must be distributed under same license terms

Examples: GNU (GPL)

*Propriertary License*

Usually strongly restrict the use, redistribution and modification of the work.

Examples: Microsoft Windows EULA, Apple MacOS license


# Software publication

1. Publication repositories (Zenodo)
2. Software journals (JOSS, JORS)
3. Method or tool section of Paper

# FAIR4RS

- *Findable* 
- *Accessible*
- *Interoperable*
- *Reusable*

- *For*
- *Research Software*

# FAIR Guidelines

- Use a publicly accessible repository with version control.
- Register your code in a community registry
- Use a software quality checklist
- Add a license
- Enable citation of the software

# Sprints

Are 1-2 weeks of focused development. They start with a planning meeting which reviews the previous sprint and select the issue to be resolved in the new sprint. The issue is broken up into smaller pieces. There are daily stand-up meetings to stay tuned. Otherwise self-organized work. Repeat until project is done. 

# Import/Effort Matrix

Defines a task from low to high impact and low to high effort. Low impact an low effort tasks should be done the last. High impact task should be priorities if they are not high effort.

# Software life cycle

1. Planning and Requirements
2. Analysis
3. Design
4. Implementation
5. Testing and Integration
6. Maintenance

# User and system requirements

*User requirements* are user centric. Helps understand context and goals of the system 

*System requirements* are developer centric. Provide technical specifications and details for building the system.

# Functional and non-functional requirements

*Functional requirements* specify behaviour and action, functionality of software systems. Can be answered with no/yes questions.

*Non-functional requierments* describe qualities or characteristics of software systems. Can't be answered wiht no/yes questions.

# MOSCOW Requirements

- *Must have*: essential, critical core functionality
- *Shoudl have*: valuable, important, but not critical
- *Could have*: nice to have, not necessary
- *Won't have*: lowest priority, out of scope

# Documenting requirements

- *Natural language*
- *Use cases*: steps and actions between actors
- *User stories*: "As a user, i want feature, so that this benefit." -> fullfilment criteria
- *Activity diagrams*: nodes (conceptual workflow steps), edges (order of execution)
- *Mockups and prototypes*

# Architectures

- *Pipeline/Workflow Architecture*: Organizes software as a series of interconnected proccesing steps. Used in data intensive software.
- *Client/Server Architecture*: Seperation of user interface and data processing and storage. Used in web aplications
- *Model-View-Controller Architecture*: Seperates application into three components. Model for data and buisness logic. View for user interfce. Controller fo input and managment of interaction of model and view.
- *Microservice Architecture*: Seperates software into a collection of small independent loosley coupled services.
- *Layered Architecture*: Seperates software into horizontal layers, where each layer performs a specific set of functions. Each layer only interact with the layers next to it.

# Programming paradigms

*Prozedual programming*

is a programming paradigm based on a sequence of instructions organized into procedures or functions that operate on data.

*Object-oriented programming*

organizes code around objects that combine data and behavior, using concepts like classes, inheritance, and encapsulation to promote modularity and reuse.

# UML Diagramms
Used in object oriented programming to get an overview how all classes connect to each other.

*Node*

1. Classname
2. Attributes
3. Methods

# Assertions
states something that must be true at a certain point in the programm. If false programm throws an error.

1. Precondition: Must be true before processing
2. Postcondition: Must be true after processing
3. Invariant: Must be true before, after and during the processing.

# Unit testing
Checks the correctness of individual components.

1. fixture: Thing being tested
2. result: Which the code produces
3. expected: To compare with result

# System testing
Testing overall functionality of the system.

# Integration testing
Testing if and how components work together.

# Regression testing
Testing when results are known. Compare results with previous results. Draws attention to changes.

# Testing floating point values

`pytest.approx()`

# Test coverage
Percentage of code which is checked by tests.

# Exceptions
Runtime error, something goes wrong while a program isrnning. In python handled with `try` and `catch`.

# Error types

- UnknownError
- ArithmeticError
- IndexError
- ValueError
- OSError

# Data Analysis Workflow
Are structured, repeatable processes used to turn raw data into meaningful insights. These workflows help ensure that your analysis is organized, efficient, and reproducible. Whether you're doing scientific research, business intelligence, or geospatial analysis, the core steps are often similar.

- In pipelines
- Often non-linear
- Can be distributed or parallel
- Implemented with workflow engines like Snakemake

# DevOps
Integrates and automates work of software development and IT operations for improving/shortening the systems development life cycle

- Containers: provide isolated and reproducible environments
- Continues Integration: AMerging incremental code changes into a main branch often.
- Conitnues Delivery: Evaluation and deployment of these incremental code changes from CI into a production environment mostly automated.







