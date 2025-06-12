#view
#  List of all Noted Video Games
```dataview
TABLE file.name AS "Title", note AS "Note", genre AS "Genre", hours_played AS "Hours", platform AS "Platform", price AS "Price"
FROM #video-games
WHERE hours_played AND platform AND price AND note AND genre
SORT note
```
