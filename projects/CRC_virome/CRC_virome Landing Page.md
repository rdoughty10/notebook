---
project:
  - CRC_virome
doc-type:
  - project page
people:
  - Ryan Doughty
---
# Project tag
#CRC_virome

# Abstract
The goal is to identify if there are bacteriophages of interest in the Gut Microbiome of CRC patients vs healthy controls

# KanBan
> Update pseudocode with this project's name and create KanBan
> 
![[CRC_virome kanban]]
# Project updates
> Add summary, thoughts, progress after presenting or completing milestone
> Include date tags with updates

# Experiments
> Update `dataview` contains() command to this project's name

```dataview
TABLE tags, date, status
WHERE contains(file.frontmatter.project, "CRC_virome")
SORT file.frontmatter.status ASC
```

# Query all notes using this project's tag
```query
#CRC_virome 
```