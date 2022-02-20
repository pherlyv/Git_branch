# Git_Branch

1. На локальном репозитории сделать ветки для:
    - Postman - `git branch Postman`.
    - Jmeter - `git branch Jmeter`.
    - CheckLists - `git branch CheckList`.
    - Bag Reports - `git branch Bug_Reports`.
    - SQL - `git branch SQL`.
    - Charles - `git branch Charles`.
    - Mobile testing - `git branch Mobile_testing`.

2. Запушить все ветки на внешний репозиторий.
    - команда `git push -u origin --all`.
4. В ветке Bag Reports сделать текстовый документ со структурой баг репорта.
- зайти в ветку `git checkout Bug_Reports`.
- создать текстовый докумет `cat > structure_bug_reports.txt`.
    - Defect ID
    - Reporter
    - Affect version
    - Project
    - Title
    - Preconditions
    - Steps of Reproduce
    - Actual result
    - Expected Result
    - Attachment
    - Severity
    - Priority
    - Environment `Enter`, `CTRL+D`.
4. Запушить структуру багрепорта на внешний репозиторий.
    - команда `git add .`.
    - команда `git commit -m "structure_bug_reports.txt"`.
    - команда `git push`.

5. Вмержить ветку Bag Reports в Main.
    - команда `git checkout main ; git merge Bug_Reports`.
6. Запушить main на внешний репозиторий.
    - команда `git add .`.
    - команда `git commit -m "merge Bug_reports"`.
    - команда `git push`.
8. В ветке CheckLists набросать структуру чек листа.
- зайти в ветку `git checkout CheckList`.
- создать текстовый документ `cat > structure_checklist.txt`.
    - List of checks
    - Environment
    - Test result `Enter`, `CTRL+D`.
10. Запушить структуру на внешний репозиторий.
    - команда `git add .`.
    - команда `git commit -m "structure_bug_reports.txt"`.
    - команда `git push`.
11. На внешнем репозитории сделать Pull Request ветки CheckLists в main.
    - зайти в ветку CheckList на github.
    - нажать кнопку `Pull Request`.
12. Синхронизировать Внешнюю и Локальную ветки Main.
    - команда `git checkout main`.
    - команда `git pull`.
