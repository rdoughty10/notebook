
# Daily Note
`="[[" + "daily_notes/" + dateformat(date(today), "yyyy") + "/" + dateformat(date(today), "MM") + "/" + dateformat(date(today), "yyyy-MM-dd") + "]]"`

> [!Tasks due today]
> 
> ```tasks
>not done
>due before tomorrow 
>```

# Projects
```dataview
TABLE project, tags, people
from "projects"
WHERE contains(file.frontmatter.doc-type, "project")
```



# What's Happening
>[!Experiments]+
>- # In-Progress
>	```dataview
>	LIST FROM "projects" and #experiment 
>	WHERE !contains(file.frontmatter.status, "complete")
>	```

# Other Tasks
>[!Pending Tasks]+
>```tasks
>not done
>limit 30
>```


>[!Recently Completed Tasks]+
>- # Alright!
>```tasks
>done
>sort by due
>limit to 10 tasks
>```


###  Lab Github Page
[tiszalab](https://github.com/tiszalab)
