# Project Milestones
Mainframe Reporting Automation Toolkit

Goal
Ship a working automation toolkit that validates, cleans, and delivers reports generated from mainframe batch jobs.

Total timeline: 8 weeks
Focus: Build → Test → Document → Ship

---------------------------------------

Week 1 — System Design

Objectives
- Understand the reporting workflow end-to-end
- Design project architecture
- Create repository structure

Tasks
[ ] Map the full pipeline (JCL → report → cleaning → SharePoint)
[ ] Define automation modules
[ ] Create GitHub repository
[ ] Set up Python environment
[ ] Create base folder structure
[ ] Write initial README draft

Deliverables
- Repo created
- Architecture notes
- Basic project structure

---------------------------------------

Week 2 — Validation Engine

Objectives
Build guardrails that detect common job configuration issues.

Tasks
[ ] Create validation module
[ ] Implement dataset existence check
[ ] Implement AP file version validation
[ ] Implement date parameter validation
[ ] Create sample config file (job_rules.yaml)

Deliverables
- validation scripts
- validation config rules

---------------------------------------

Week 3 — Report Cleaning Engine

Objectives
Replace manual Excel cleanup with automated processing.

Tasks
[ ] Build report parser
[ ] Normalize column headers
[ ] Remove blank or invalid rows
[ ] Add data validation checks
[ ] Generate cleaned output file

Deliverables
- cleaning module
- sample cleaned report output

Libraries
Python
pandas

---------------------------------------

Week 4 — Pipeline Runner

Objectives
Connect validation and cleaning into one workflow.

Tasks
[ ] Create pipeline runner script
[ ] Add CLI interface
[ ] Implement workflow steps
    validate → clean → generate output
[ ] Add logging for pipeline steps

Deliverables
- working pipeline script
- CLI command to run full process

Example
python run_pipeline.py --input report.txt

---------------------------------------

Week 5 — SharePoint Integration

Objectives
Automate report delivery.

Tasks
[ ] Research SharePoint upload API
[ ] Implement SharePoint authentication
[ ] Create upload module
[ ] Upload processed reports automatically

Deliverables
- sharepoint_uploader module
- successful test upload

---------------------------------------

Week 6 — Pipeline Integration

Objectives
Connect the uploader with the pipeline.

Tasks
[ ] Add SharePoint upload step to pipeline
[ ] Add error handling
[ ] Implement retry logic
[ ] Add configuration options

Deliverables
- fully automated pipeline

Pipeline Flow
mainframe report → validation → cleaning → upload

---------------------------------------

Week 7 — Documentation

Objectives
Explain the system clearly.

Tasks
[ ] Write architecture documentation
[ ] Create workflow diagrams
[ ] Document modules
[ ] Add setup instructions
[ ] Add example dataset

Deliverables
- docs folder
- architecture.md
- workflow diagram

---------------------------------------

Week 8 — Release and Demo

Objectives
Ship the project publicly.

Tasks
[ ] Clean up code
[ ] Improve README
[ ] Record demo walkthrough
[ ] Publish GitHub repo
[ ] Share project on LinkedIn

Deliverables
- public GitHub project
- demo explanation
- portfolio-ready project

---------------------------------------

Final Outcome

A working automation toolkit that demonstrates:

- enterprise reporting pipeline automation
- data validation
- data cleaning
- system integration
