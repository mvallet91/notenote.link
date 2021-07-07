---
title: PhD Proposal Public
season: summer
tags: CMS
---

## PhD Proposal

### Background
Sequential Pattern Mining has been studied since the 90s ([[agrawal1994fast]]), when it was introduced as an algorithm to find association rules: if a set of consequent items is present in multiple groups, regardless of other items that may be included in the groups. It has been applied to learning for more than 10 years, for instance using nStudy to find patterns in learner interaction with multimedia learning environments ([[zhou2010sequential]]), with more recent efforts focusing on developing knowledge- and theory-derived features as the units of sequences ([[wang2021automating]], [[lamsa2020potential]]). Most of these works investigate sequences and patterns as a descriptive analysis after a study or course, from a researcher or teacher perspective. The goal of this work is to research how we can use it to support learners and close the feedback cycle ([[hattie2007power]]) in different stages.

### Opportunity & Approach
The idea is to look into sequences of actions, using Sequential Pattern Mining (SPM) or Sequence Analytics; but also considering the temporality of the actions, with approaches such as Lag Sequential Analysis (LSA - what happens between patterns) ([[lamsa2020potential]], [[chen2020mining]]) and Response-Time Decomposition (RTD - what happens between actions within a task) ([[gurung2021decomposition]]) and use them to:
- Use theory- and knowledge-driven features to generate students' action sequences when working on formal domains such as math, physics or programming
- Study different levels of sequences: 
	1. In the current task
	2. Their general approach to assignments
	3. Interaction with all (online) materials throughout a course 
- Experiment with different methods of sequential and temporal analysis to find patterns in these sequences
- Find groups or clusters of patterns 


**Short feedback cycles:** 
- Find the patterns that lead to success within different groups, and use them provide automatic feedback to similar students ([[perera2009clustering]])
- Assist teachers to provide feedback to the groups of each pattern, facilitating specific feedback to a greater number of students ([[bernius2021machine]])
	
**Medium & Long Feedback Cycles**
- Explore the support of Self-Regulated Learning ([[zimmerman2009self]]) with Sequence Pattern Mining to assess the level of each student ([[fan2021learning]] , [[manso2018xapi]]), with contextual features such as their previous experience or general level ([[kinnebrew2013contextualized]]) and provide support, from simple prompts to sequence visualizations:
	- For relevant processes, like abcdeSIM ([[faber2018game]]), create a report with timeline visualizations for self-reflection - Map the learner actions, system responses, and other references (expected deadlines, peer or group sequences, etc) to time, then portray it as a review so students can explore and reflect on their own process ([[vazquezbarreiros2014softlearn]], [[valle2020edx]] )
- **Interoperability** - Evaluate the benefits of using xAPI to continue the initiative for interoperability and easier transfer of efforts for wider studies/implementations ([[bakharia2016recipe]] , [[manso2018xapi]]). Look into the use of a generic logging tool, like LogUI ([[maxwell2021logui]] ), to generate own logs, instead of depending on those provided by the different platforms. 
- 
#proposal-ref

### References
```dataviewjs

let refs = dv.array(dv.pages("#proposal-ref").file.outlinks)
dv.list(
	refs.map(r => [
		r, dv.page(r.path).title,  dv.page(r.path).authors
	])
)
```