echo "# название" >> README.md

**git init** - _инициализация пустого репозитория_

**git add README.md** - _добавляет содержимое рабочего каталога в индекс (staging area) для последующего коммита_

**git commit -m "first commit"** - _сохраняет их слепок во внутренней базе данных, а затем сдвигает указатель текущей ветки на этот слепок_

**git remote add origin https://github.com/LutovinovKN/название.git** - \*\*

**git push -u origin master** - \*\*

**git log --oneline** - _посмотреть все коммиты_

**git checkout .** - _восстановить все_

**git checkout "код коммита"** - _вернуть до состояния этого коммита_

**git checkout master** - _вернуться в ветку мастер_

## Восстановить файлы на локальном компьютере:

**git fetch --all**

**git reset --hard origin/master или git reset --hard origin/<название_ветки>**

**git add text.txt** - _добавить файл в репозиторий_

**git rm text.txt** - _удалить файл_

**git status** - _Текущее состояние репозитория (изменения, неразрешенные конфликты и тп)_

**git commit -a -m "Commit description"** - _Сделать коммит_

**git push origin** - _Замерджить все ветки локального репозитория на удаленный репозиторий_

**git push origin master** - _Аналогично предыдущему, но делается пуш только ветки master_

**git push origin HEAD** - _Запушить текущую ветку, не вводя целиком ее название_

**git pull origin** - _Замерджить все ветки с удалённого репозитория_

**git pull origin master** - _Замержить только ветку master с удалённого репозитория_

**git pull origin HEAD** - _Накатить текущую ветку, не вводя ее длинное имя_

**git fetch origin** - _Скачать все ветки с origin, но не мерджить их в локальный репозиторий_

**git fetch origin master** - _Аналогично предыдущему, но только для одной заданной ветки_

**git checkout -b some_branch origin/some_branch** - _Начать работать с веткой some_branch (уже существующей)_

**git branch some_branch** - _Создать новую ветку (ответвится от текущего)_

**git checkout some_branch** - _Переключиться на другую ветку (из тех, с которыми уже работаем)_

**git branch** - _(звездочкой отмечена текущая ветвь) - Получаем список веток, с которыми работаем_

**git branch -a # | grep something** - _Просмотреть все существующие ветви_

**git merge some_branch** - _Замерджить some_branch в текущую ветку_

**git branch -d some_branch** - _Удалить замерженную ветку (после мерджа)_

**git branch -D some_branch** - _Просто удалить ветвь (тупиковая ветвь)_

**git show bf20199debfde53a5cd09a19fc4fc055138ad6c4** - _Изменения, сделанные в заданном коммите_

**git push origin :branch-name** - _Удалить ветвь из репозитория на сервере_

**git reset --hard bf20199debfde53a5cd09a19fc4fc055138ad6c4** - _Откатиться к конкретному коммиту и удалить последующие (хэш смотрим в «git log»)_

**git push -f** - _залить на сервер измененные коммиты_

**git clean -f** - _Удаление untracked files_
