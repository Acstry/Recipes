### Breakfast
```dataview
LIST FROM #breakfast SORT file.name asc
```
### Appetizers
```dataview
LIST FROM #appetizer SORT file.name asc
```
### Meals
```dataview
LIST FROM #meal SORT file.name asc
```
### Desserts
```dataview
LIST FROM #dessert SORT file.name asc
```
### Sauces
```dataview
LIST FROM #sauce SORT file.name asc
```
### Extras
```dataview
LIST FROM #component SORT file.name asc WHERE !contains(file.tags, "part") and !contains(file.tags, "sauce")
```