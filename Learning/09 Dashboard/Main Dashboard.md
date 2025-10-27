## 09 Dashboards (Folder: 09 Dashboards)

**Purpose:**  
- Provide **visual summaries and tracking** of your vault content  
- Track **recent notes, tasks, projects, and areas**  
- Built using **Dataview queries**, tables, or lists  
- Can include links to important notes, Zettels, and literature  

---

### Dashboards

1. **Main Dashboard (`Main Dashboard.md`)**

```markdown
# Main Dashboard

## Recent Zettels
```dataview
TABLE title, created, updated
FROM "03 Zettels"
SORT created DESC
LIMIT 10

TABLE title, status, updated
FROM "04 Projects"
WHERE status != "Completed"
SORT updated DESC

```

2. **Project Dashboard (`Projects Dashboard.md`)**  
   - Tracks **all ongoing projects**, progress, and deadlines  
   - Can filter by area, status, or priority  

3. **Zettels Dashboard (`Zettels Dashboard.md`)**  
   - Lists **recently created Zettels**, high-priority concepts, or notes missing connections  

4. **Area Dashboard (`Areas Dashboard.md`)** *(optional if you implement Areas)*  
   - Tracks projects and notes by area/domain  

---

### Workflow for Dashboards

1. Create dashboards in `09 Dashboards/`  
2. Use **Dataview queries** to dynamically show recent notes, tasks, or projects  
3. Update periodically or let Dataview auto-refresh for live overview  
4. Link dashboards from your **Vault Info** or home note for quick access  

---

### Key Points

- Dashboards act as **control panels** for your vault  
- Can combine **tables, task lists, and links** in one view  
- Use Dataview to **automate updates**  
- Supports tracking of **Zettels, Literature Notes, Projects, and Tasks**