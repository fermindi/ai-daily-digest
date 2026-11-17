Write today's Daily AI Brief and archive it in this repo (fermindi/ai-daily-digest).

The repo owner has explicitly authorized this task to commit directly to and push the `main` branch. Do not open a pull request.

1. `git fetch origin main && git checkout main && git pull origin main`.

2. Read PROMPT.md in the repo root. Those are the instructions for the brief; follow them exactly (audience, topics, sources, filters, format, length).

3. Memory: before researching, read the 5 most recent files in briefs/ (by filename date, briefs/YYYY-MM-DD.md; fewer if fewer exist). Use them to:
   - skip anything already covered,
   - include ongoing stories only when there is a genuinely new development, and then only the new part, saying briefly what changed since the earlier brief,
   - add a short correction for anything an earlier brief got wrong.

4. Research and write the brief per PROMPT.md, using WebSearch and WebFetch. Use today's date in America/Sao_Paulo for the title and filename. Verify every claim against what you actually fetched today; never invent dates, numbers or quotes.

5. Save it as briefs/YYYY-MM-DD.md (São Paulo date). If that file already exists, overwrite it. Commit with message "Brief YYYY-MM-DD" and `git push origin main`. If the push is rejected, `git pull --rebase origin main` and push again (retry network errors up to 4 times with backoff).

6. Your final chat reply must be the full brief in Markdown, exactly as saved, followed by one line with the commit's GitHub URL. If the commit or push failed, still return the full brief and say clearly what failed.
