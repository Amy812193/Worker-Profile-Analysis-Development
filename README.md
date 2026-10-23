# Worker Profile Analysis & Development
Buiding AI course project

## Summary

This tool analyses CVs to identify strengths, areas for improvement, core and secondary areas of expertise, and transferable skills, helping job seekers position their profile and focus their search. For people already in a role, it highlights the future skills their field will need and recommends training and certifications to strengthen their profile. 


## Background

- Many people can’t clearly name their strengths or transferable skills, or present them well on a CV. People in work often don’t know which future skills or training to invest in, and career coaching can be expensive and hard to access.

- By 2030, 39% of core job skills are expected to change, and 59% of the global workforce will need training (World Economic Forum, [The Future of Jobs Report 2025](https://www.weforum.org/publications/the-future-of-jobs-report-2025/), January 2025)

- The tool will help people find jobs faster, opens up career changes, and points training spending where it pays off. It also makes personalised career guidance available to everyone at a time when skills are changing fast.


## How is it used?

The tool is a self-service web application.

Job seekers use it to improve their CV and focus their search and job workers to plan their career development.


## Data sources and AI methods

The main data source is the user’s CV, uploaded as a PDF or Word file, or imported from a LinkedIn profile. The tool extracts its key elements (skills, job titles, job descriptions, education and training) and maps them to ESCO (European Skills, Competences, Qualifications and Occupations) to classify them in a standard way.

For the job market, the tool analyses job postings from job boards to identify which skills are currently in demand. It also draws on recent labour market reports to describe the skills that will matter in the future.

For training, the tool connects to course platforms and certification catalogues to suggest options that fit the user’s profile.

Users can also enter keywords describing the direction they want to take their career, so the suggestions match their goals.

AI techniques

The skill mapping will use embeddings and semantic similarity match free-text skills to ESCO entries, even when the wording differs.
The matching and recommendation will be based on a similarity score between the profile and job roles identifies the core area, secondary areas and transferable skills, and points to training that fills the gaps.
The trend analysis will use job posting data over time to spot emerging skills.
The large language models will summarise strengths and areas for improvement, explain recommendations in plain language, and suggest how to position the profile.


## Challenges

The tool itself will face 2 main challenges:

- Unstructured CVs: CV formats and wording vary widely. The tool extracts the relevant information and classifies it against ESCO. When a match is uncertain, it suggests the closest equivalent terms for the user to confirm.
- GDPR compliance: the tool asks for explicit consent before processing, anonymises CVs, keeps data only for as long as necessary, and lets users delete their profile at any time.

For users, the main risk is biased assessment, which could affect people with atypical career paths, people with low digital skills and older workers. The tool should therefore always offer suggestions and alternatives, rather than rewriting profiles.


## What next?

The tool could evolve from a CV analysis tool into a complete career companion that supports users over time. This would involve wider partnerships with job boards, LinkedIn, training platforms and public employment services.


## Acknowledgments

- Applicant Tracking System (ATS) software, which inspired this project: applying the same logic, but in reverse, to support job seekers and employed professionals
- [Elements of AI](https://www.elementsofai.com/), for providing a framework to structure the project and explain the methodology behind AI
