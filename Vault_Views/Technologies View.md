#view 

# List of All technologies Documented group by types
```dataview
TABLE file.name AS "Technology", devops AS "Devops", technology AS "Type"
FROM #technology 
SORT technology DESC
```

# List only the DevOps technologies
```dataview
TABLE file.name AS "Technology", devops AS "Devops", technology AS "Type"
FROM #technology 
WHERE devops = "✅"
SORT technology DESC
```
