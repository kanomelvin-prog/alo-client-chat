# Alo Client Chat
   
   Live at: https://withalo.me
   
   ## Versions
   - `index.html` - Current live version
   - `versions/` - Timestamped backups
   
   ## History
   See version files for dated backups
```

4. **Your structure in each repo:**
```
   alo-client-chat/
   ├── index.html              ← Current live version
   ├── versions/
   │   ├── baseline_20251229.html
   │   └── (future versions here)
   └── README.md
   
   alo-dashboard/
   ├── index.html              ← Current live version
   ├── versions/
   │   ├── baseline_20251229.html
   │   └── (future versions here)
   └── README.md
```

---

## Testing URLs

After you create the versions folder:

- **Live chat:** `https://withalo.me/index.html` (or just `https://withalo.me`)
- **Baseline backup:** `https://withalo.me/versions/baseline_20251229.html`

Same pattern for dashboard.

---

## Quick Workflow Moving Forward

**When making changes:**

1. **Before editing `index.html`:**
```
   Click "Add file" → "Create new file"
   Name: versions/backup_20251229_1030.html
   Paste current index.html code
   Commit: "Backup before Supabase integration"
```

2. **Edit `index.html` directly**
   - Make your changes
   - Commit with clear message

3. **If it works:**
```
   Create: versions/supabase-working_20251229.html
   Copy the working index.html
   Commit: "Supabase integration working"
```

4. **If it breaks:**
```
   Go to versions/baseline_20251229.html
   Click "Raw"
   Copy all code
   Edit index.html
   Paste copied code
   Commit: "Rollback to baseline"
