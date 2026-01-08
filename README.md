# Over-The-Wire-Journey
My solutions and learnings from completing the Bandit wargame.

## Progress
- ✅ Levels 0-33 completed on 1/7/2026

## Key Learnings

### Level Categories
- **File Permissions & Commands** (Levels 1-5)
- **Networking** (Levels 15-16, 20-21)
- **Cron Jobs** (Levels 21-24)
- **Git & Version Control** (Levels 27-31)
- **Shell Escaping** (Levels 25-26, 32)

### Tools Mastered
- SSH & SCP
- netcat, nmap
- openssl
- git (branches, tags, commits)
- vim
- bash scripting

## Levels That Were Particularly Challenging

### Level 12→13: Hexdump Decompression
**Challenge:** Getting through multiple layers of compression
**Solution:** Once I got the first decompressed file of each type, it became a pattern of repeating the decompression process
**Key Takeaways:** Repetition is useful in CTF challenges, and tasks get easier the further along you go. Understanding file types and compression formats is essential.

### Level 15→16: SSL/TLS Connection
**Challenge:** Submit password via SSL to localhost:30001
**Solution:** Used `openssl s_client -connect localhost:30001 -ign_eof` to establish an encrypted connection
**Key Takeaway:** Understanding encrypted connections and how to work with SSL/TLS protocols

### Level 25→26: Terminal Manipulation & Vim Escape
**Challenge:** Breaking out of a restricted shell that immediately logs you out
**Solution:** Resized terminal to trigger the `more` pager, pressed `v` to enter vim, then used `:set shell=/bin/bash` and `:shell` to escape
**Key Takeaways:** Creative problem-solving with terminal behavior and understanding how pagers work

### Level 27→33: Git & Version Control
**Challenge:** Finding layered passwords hidden in git history, branches, tags, and dealing with .gitignore
**Solution:** Used `git log`, `git show`, `git checkout`, `git tag`, and learned to configure git identity for commits and pushes
**Key Takeaways:** Deep understanding of git internals, how version control stores information, and how to navigate repository history

## Reflections
Completing all 33 levels taught me the importance of persistence, reading documentation, and thinking creatively about problem-solving in cybersecurity contexts.
