---
project: 
doc-type:
  - project page
people:
---
# Project tag
> make a unique tag for all experiments/analyses and add it to queries/dataviews 

#mft

# Abstract
Making things more sensitive

# KanBan
> Update pseudocode with this project's name and create KanBan
![[MFT kanban]]
# Project updates
> Add summary, thoughts, progress after presenting or completing milestone
> Include date tags with updates

# Experiments
> Update `dataview` contains() command to this project's name

```dataview
TABLE tags, date, status
WHERE contains(file.frontmatter.project, "projectname")
SORT file.frontmatter.status ASC
```

# Query all notes using this project's tag
```query
#projectname
```