- What did you put in your `CLAUDE.md`, and what did you deliberately leave out, and why?

I had nothing to add to the file , I removed the detail at the top as we know already this is for a tutorial

- Which permission rules did you add, and what could go wrong without your deny rule?

    "allow": ["Bash(npm test:*)"],
    "ask": ["Bash(git push:*)"],
    "deny": ["Read(./.env)", "Bash(git push --force:*)"]

    The deny rule could be a problem if we change the PORT as we use that variable. claude may not know what port it actually runs on at that point.


I used /memory and could see the claude.md loaded.

I used /permissions and could see the permissions from the settings.json were active