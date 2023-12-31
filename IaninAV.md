# Руководство пользователя по GIT
## 1. Основные команды
* *git init* - инициализирует локальный репозиторий
* *git add filename* - помечает файл с именем ***filename*** на включение в следующий коммит
* *git commit*
* * *git commit -m "Description"* - создает коммит c описанием ***Description***
* * *git commit -am "Description"* - создает коммит c описанием ***Description*** и включением отслеживаемых файлов в будущий коммит
* *git merge branch_name* - выполняет слияние из ветки ***branch_name*** в текущую ветку
## 2. Работа с ветками
* *git branch* - выводит спиcок веток
* *git branch branch_name* - создает новую ветку с именем ***branch_name***
* *git branch -d branch_name* - удаляет ветку с именем ***branch_name***
## 3. Переключения между коммитами и ветками
* *git checkout branch_name* - переключится на ветку с именем ***branch_name***
* *git checkout commits_hash* - переключится на коммит с хэшем ***commits_hash***
* *git checkout -b branch_name* - переключится на ветку с именем ***branch_name*** предвартельно создав ее
## 4. Информационные команды
* *git status* - получить информацию о текщем состоянии
* *git log* - вывод на экран истории всех коммитов с их хэш-кодами
* *git log --graph* - вывод на экран истории всех коммитов с их хэш-кодами со взаимосвязями в более нагдядном виде
* *git diff* - показывает разницу между коммитами
## 5. Команды удаления
* *git reset --hard commits_hash~* - удаляет коммит с указанным хэшем
## 6. Команды работы с удаленным репозиторием
* *git clone web_repository_address* - создает копию удаленного репозитория с адресом ***web_repository_address*** в локальном репозитории
* *git push* - синронизирует данные с локального репозитория на связанный удаленный репозиторий
* *git push* --set-upstream origin branch_name - синхронизирует новую ветку ***branch_name*** с локального репозитория на удаленный репозиторий с отслеживанием
* *git push --all* - синхронизирует все ветки с локального репозитория на связанный удаленный репозиторий
* *git pull* - синронизирует данные с удаленного репозитория на связанный локальный репозиторий
* *git remote add name web_repository_address* - добавляет удаленный репозиторий с именем ***name*** по адресу ***web_repository_address***