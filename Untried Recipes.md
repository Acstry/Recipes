```dataview
LIST FROM #meal SORT file.name asc
WHERE contains(file.tags, "untried")
flatten file.name
```

