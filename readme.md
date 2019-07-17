# Git pull hook
## For Laravel 5
![A preview](git-pull-hook.png)

---
### Информация
Данный хук после `git pull` или `git merge`, уведомляет об изменениях в зависимостях (composer, npm) и миграциях.

Можно запускать команды автоматически (напр. `php artisan migrate`), если раскомментировать строчки в файле `post-merge`

### Установка
 - Файл `post-merge` переместить в папку `.git/hooks/`
 - Дать файлу `post-merge` права на исполнение: `chmod +x post-merge` | `chmod +x .git/hooks/post-merge`
