# Git Руководство пользователя
## 1. Основные команды
* git init - инициализирует локальный репозиторий
* в самом начале перед работой в папке обязательно git add и папка, обычно Tab
* Далее используем git commit -am сохраняет и добаляет комментарий 
* git commit -m - Просто добавляет комментарий
* git log - просмотр commit
* git checkout - чтобы вернуться в commit
* git checkout master (наименование ветки) - возвращает в актуальную версию
 git reset HEAD~ - удаление последнего commit
 *  git reset --hard HEAD~ - удаление commit и всех изменений с ним
 * git status - узнать статус
 ## 2. Работа с ветками
 * git branch - выводит список веток
 * git branch name - создает ветку с именем name
 * git branch -D - удаление ветки
 * git merge - выполняет слияние веток
 * git config --global user.name - для написания совего имени для git
 * git config --global user.email - для написания соего email для git
 * git diff - список изменений внесенный в репозиторий
 * git commit --amend -m - дает возможность редактировать сообщение commit
 * git revert HEAD - откат последнего commit
 * git log --all - для просмотра исотрии commit по всем веткам