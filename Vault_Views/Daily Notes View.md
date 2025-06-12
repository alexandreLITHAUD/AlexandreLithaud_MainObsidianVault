#view
# Average Mood for my Daily Notes globally
```dataview
TABLE WITHOUT ID
round(average(number(mood)), 2) as "Average Mood / 10"
FROM #dailynote
WHERE mood
```

# Average Mood this Week
```dataview
TABLE WITHOUT ID
round(average(number(mood)), 2) as "Average Mood / 10 (Last 7 Days)"
FROM #dailynote 
WHERE mood AND file.ctime >= date(today) - dur(7 days)
```


