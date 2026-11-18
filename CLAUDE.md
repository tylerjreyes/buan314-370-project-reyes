# Project rules

This is a course project in exploratory data analysis. I am the analyst and decision-maker. You write and run the code. I am not a programmer, so explain what you did in plain English.

## Tools
- Language: R for all data work, analysis, models and figures. Do not switch languages.
- Visualizations are prototyped with any plotting library in that language. The finished versions are saved by the numbered scripts, and those files are the ones used in the LaTeX report and in the slides. Quick trials go in the scratch folder (scratch/).
- The HTML report shows the same visualizations, rebuilt in its own CSS and JavaScript. Do not paste image files into it.
- The static report is LaTeX, compiled in Overleaf.
- The interactive report is one hand-written HTML file with its CSS and JavaScript inside it. No page generators, no notebooks exported to HTML, no libraries loaded from the web.
- Use paths relative to the project folder. Set a seed wherever anything is random.

## Data
- Never change, rename or delete anything in data/raw.
- Every change to the data happens in a numbered script in scripts/, never by hand and never in a one-off command.
- Never drop rows, drop columns, fill in missing values or recode categories unless I have approved that specific step.

## Documentation (do this without being asked)
- After any step that changes rows or columns, add a row to documentation/wrangling_log.md: step number, what changed, why, rows before, rows after, script name.
- Whenever a variable is created, renamed or recoded, update documentation/codebook.md.
- After each prompt, add an entry to documentation/prompt_log.md: date, my prompt as I wrote it, a one-line summary of what you did, the files you changed.
- Take variable definitions from the source's data dictionary. If something is undocumented, write UNDOCUMENTED. Do not guess.

## Models
- Models are ordinary linear regressions only, fitted on all rows of the processed data. That includes the classification problem, which uses a linear probability model. Do not use any other kind of model. Do not split the data or choose variables automatically.

## Results
- Report numbers and where you saved them. Give the count behind every average and percentage.
- Do not interpret findings or write conclusions for me unless I ask.

## Git and safety
- Ask before installing software, deleting any file, or creating anything on GitHub.
- No passwords, keys or personal information in any file.
- When a step is finished and checked, commit with a message that says what changed and why, then push. Never rewrite history.
