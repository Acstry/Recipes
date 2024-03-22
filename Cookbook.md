### Breakfast
```dataview
LIST FROM #breakfast SORT file.name asc
flatten file.name
```
---
### Appetizers
```dataview
LIST FROM #appetizer SORT file.name asc
flatten file.name
```
---
### Meals
```dataview
LIST FROM #meal SORT file.name asc
flatten file.name
```
---
### Desserts
#### Cakes
```dataview
LIST FROM #cake SORT file.name asc
flatten file.name
```
#### Cookies
```dataview
LIST FROM #cookie SORT file.name asc
flatten file.name
```
#### Others
```dataview
LIST FROM #dessert SORT file.name asc WHERE !contains(file.tags, "cookie") and !contains(file.tags, "cake")
flatten file.name
```
---
### Sauces
```dataview
LIST FROM #sauce SORT file.name asc
flatten file.name
```
---
### Extras
```dataview
LIST FROM #component SORT file.name asc WHERE !contains(file.tags, "part") and !contains(file.tags, "sauce")
flatten file.name
```