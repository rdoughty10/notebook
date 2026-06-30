---
project:
  - proj1
doc-type:
  - project page
people:
  - Wayne
---
# Project tag
> make a unique tag for all experiments/analyses and add it to queries/dataviews 

#proj1

# Abstract
> Brief summary of the **why** and **how** of this project

# KanBan
> Update pseudocode with this project's name and create KanBan

![[projects/proj1/proj1 kanban]]
# Project updates
> Add summary, thoughts, progress after presenting or completing milestone
> Include date tags with updates

# Experiments
> Update `dataview` contains() command to this project's name

```dataview
TABLE file.tags, file.frontmatter.date AS "date", file.frontmatter.status AS "status"
WHERE contains(file.frontmatter.project, "proj1")
and contains(file.frontmatter.doc-type, "experiment")
SORT file.frontmatter.status ASC
```

# Query all notes using this project's tag
> update query code to use this project's tag

```query
#proj1
```