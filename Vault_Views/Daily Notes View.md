#view
# Average Mood for my Daily Notes globally
```dataview
TABLE mood AS "Mood"
FROM #dailynote
WHERE mood
```

# Average Mood this Week
```dataview
TABLE mood AS "Mood"
FROM #dailynote 
WHERE mood AND file.ctime >= date(today) - dur(7 days)
```
