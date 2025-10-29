
### Recent Zettels
```dataview
TABLE title, created, updated
FROM "03 Zettels"
SORT created DESC
LIMIT 10


TABLE title, status, updated
FROM "04 Projects"
WHERE status != "Completed"
SORT updated DESC

TASK FROM "01 Inbox" OR "04 Projects"
WHERE !completed

TABLE title, tags
FROM ""
WHERE contains(tags, "Math")
