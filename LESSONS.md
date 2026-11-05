# Lessons

- Asked in Spanish, user switched to "answer in english" → reply in English unless told otherwise.
- Column case differs by dataset: jobs_class.cvs is UPPERCASE (YEAR, POOR); firmsize_clean_data.csv is lowercase (year, asecwt) → check the dataset's real columns first.
- Told user to reopen Colab GitHub link after push; Colab served cached old version → give a commit-pinned Colab link (blob/<full SHA>/) after each push.
- Built graphs on old jobs_class.cvs; user wanted firmsize_clean_data.csv from Firmsize_CPS_data_prep_1996_2026.ipynb → git fetch main and read the latest prep notebook before choosing a dataset.
- Final Colab notebooks and graphs go to My Drive/Jobs, Workers, and Development/Project.
- Colab popup "No se pudo enviar el mensaje al entorno de ejecución: TypeError: Load failed" = browser lost connection to the runtime (Safari), not a code bug → reload, reconnect runtime, or use Chrome.
- KeyError firmsize4_label: Drive CSV was an older prep version → user wants exactly 4 firm-size groups (under 10, 10-99, 100-499, 500+); stop with a clear 're-run the prep notebook' message instead of falling back to 3 groups.
- Prep used range(1996, 2026), which stops at 2025; user wants 1996-2026 → range end is exclusive, use range(1996, 2027) and check years in the data.
- User dislikes graphs that pool all years (graphs 1, 7-10) → compare snapshot years 1996, 2006, 2016, 2026, one panel per year side by side.
