# Домашнее задание к занятию "`Системы контроля версий`" - `Тен Денис`


### Цель задания

В результате выполнения задания вы: 

* научитесь подготоваливать новый репозиторий к работе;
* сохранять, перемещать и удалять файлы в системе контроля версий.  


### Чеклист готовности к домашнему заданию

1. Установлена консольная утилита для работы с Git.


### Инструкция к заданию

1. Домашнее задание выполните в GitHub-репозитории. 
2. В личном кабинете отправьте на проверку ссылку на ваш репозиторий с домашним заданием.
3. Любые вопросы по решению задач задавайте в чате учебной группы.


### Дополнительные материалы для выполнения задания

1. [GitHub](https://github.com/).
2. [Инструкция по установке Git](https://git-scm.com/downloads).
3. [Книга про  Git на русском языке](https://git-scm.com/book/ru/v2/) - рекомендуем к обязательному изучению главы 1-7.
   

------

## Задание 1. Создать и настроить репозиторий для дальнейшей работы на курсе

В рамках курса вы будете писать скрипты и создавать конфигурации для различных систем, которые необходимо сохранять для будущего использования. 
Сначала надо создать и настроить локальный репозиторий, после чего добавить удалённый репозиторий на GitHub.

### Создание репозитория и первого коммита

1. Зарегистрируйте аккаунт на [https://github.com/](https://github.com/). Если предпочитаете другое хранилище для репозитория, можно использовать его.
2. Создайте публичный репозиторий, который будете использовать дальше на протяжении всего курса, желательное с названием `devops-netology`.
   Обязательно поставьте галочку `Initialize this repository with a README`. 

  ![Диалог создания репозитория](https://raw.githubusercontent.com/netology-code/sysadm-homeworks/devsys10/02-git-01-vcs/img/github-new-repo-1.jpg)
    
3. Создайте [авторизационный токен](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) для клонирования репозитория.
4. Склонируйте репозиторий, используя протокол HTTPS (`git clone ...`).
 
    ![Клонирование репозитория](https://github.com/netology-code/sysadm-homeworks/blob/devsys10/02-git-01-vcs/img/github-clone-repo-https.jpg)




6. Перейдите в каталог с клоном репозитория (`cd devops-netology`).
7. Произведите первоначальную настройку Git, указав своё настоящее имя, чтобы нам было проще общаться, и email (`git config --global user.name` и `git config --global user.email johndoe@example.com`). 
8. Выполните команду `git status` и запомните результат.
9. Отредактируйте файл `README.md` любым удобным способом, тем самым переведя файл в состояние `Modified`.
10. Ещё раз выполните `git status` и продолжайте проверять вывод этой команды после каждого следующего шага. 
11. Теперь посмотрите изменения в файле `README.md`, выполнив команды `git diff` и `git diff --staged`.
12. Переведите файл в состояние `staged` (или, как говорят, просто добавьте файл в коммит) командой `git add README.md`.
13. И ещё раз выполните команды `git diff` и `git diff --staged`. Поиграйте с изменениями и этими командами, чтобы чётко понять, что и когда они отображают. 
14. Теперь можно сделать коммит `git commit -m 'First commit'`.
15. И ещё раз посмотреть выводы команд `git status`, `git diff` и `git diff --staged`.

## Выполнение Задание 1. Создать и настроить репозиторий для дальнейшей работы на курсе

1. Зарегистрируйте аккаунт на [https://github.com/](https://github.com/). Если предпочитаете другое хранилище для репозитория, можно использовать его.
2. Создайте публичный репозиторий, который будете использовать дальше на протяжении всего курса, желательное с названием `devops-netology`.
   Обязательно поставьте галочку `Initialize this repository with a README`.
   
![Создание репозитория](https://github.com/user-attachments/assets/857dc479-2fb4-4b71-9e09-00dabdf467ed)

3. Создайте [авторизационный токен](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) для клонирования репозитория.

![Создание авторизационного токена](https://github.com/user-attachments/assets/9947af65-53b1-42ed-b0fe-f3334aa107eb)

4. Склонируйте репозиторий, используя протокол HTTPS (`git clone ...`).
![Клонирование репозитория](https://github.com/user-attachments/assets/2d2295f3-64a1-41a6-8f05-1587738ecb70)

```bash
git clone https://github.com/killakazzak/devops-netology.git
```

![image](https://github.com/user-attachments/assets/cedfebdd-420e-4a14-848a-0f8a7b50e36b)


6. Перейдите в каталог с клоном репозитория (`cd devops-netology`).
   
![image](https://github.com/user-attachments/assets/64d3954a-2334-479e-9e48-3584033e5323)

7. Произведите первоначальную настройку Git, указав своё настоящее имя, чтобы нам было проще общаться, и email (`git config --global user.name` и `git config --global user.email johndoe@example.com`).

```bash
git config --global user.name "Denis Ten"
git config --global user.email denis.a.ten@gmail.com
git config --list --show-origin
```
![image](https://github.com/user-attachments/assets/e645e15c-5d84-4612-86db-6eea257ebe89)


8. Выполните команду `git status` и запомните результат.

```bash
git status
```
![image](https://github.com/user-attachments/assets/4a461287-4a04-4167-a736-17ac1bd096e7)

9. Отредактируйте файл `README.md` любым удобным способом, тем самым переведя файл в состояние `Modified`.
10. Ещё раз выполните `git status` и продолжайте проверять вывод этой команды после каждого следующего шага. 

![image](https://github.com/user-attachments/assets/cf3bfe1b-22e2-482e-831a-7b4a73be8805)

11. Теперь посмотрите изменения в файле `README.md`, выполнив команды `git diff` и `git diff --staged`.
```bash
git diff
git diff --staged
```
![image](https://github.com/user-attachments/assets/d20b018c-7d54-44f2-9d5e-871716a48b76)

12. Переведите файл в состояние `staged` (или, как говорят, просто добавьте файл в коммит) командой `git add README.md`.
13. И ещё раз выполните команды `git diff` и `git diff --staged`. Поиграйте с изменениями и этими командами, чтобы чётко понять, что и когда они отображают.

```bash
git add README.md
git diff
git diff --staged
```

![image](https://github.com/user-attachments/assets/06ed66f5-f889-4555-a566-a2457f81d543)

14. Теперь можно сделать коммит `git commit -m 'First commit'`.
15. И ещё раз посмотреть выводы команд `git status`, `git diff` и `git diff --staged`.

```bash
git commit -m 'First commit'
git diff
git diff --staged
```

![image](https://github.com/user-attachments/assets/f0ade6db-3bf1-4b4c-9637-c8304d7fc547)

```bash
git status
```
![image](https://github.com/user-attachments/assets/c5c06233-37cf-4360-8808-7d561896f51a)


### Создание файлов `.gitignore` и второго коммита

1. Создайте файл `.gitignore` (обратите внимание на точку в начале файла), проверьте его статус сразу после создания. 
1. Добавьте файл `.gitignore` в следующий коммит (`git add...`).
1. На одном из следующих блоков вы будете изучать `Terraform`, давайте сразу создадим соотвествующий каталог `terraform` и внутри этого каталога — файл `.gitignore` по примеру: https://github.com/github/gitignore/blob/master/Terraform.gitignore.  
1. В файле `README.md` опишите своими словами, какие файлы будут проигнорированы в будущем благодаря добавленному `.gitignore`.
1. Закоммитьте все новые и изменённые файлы. Комментарий к коммиту должен быть `Added gitignore`.

### Эксперимент с удалением и перемещением файлов (третий и четвёртый коммит)

1. Создайте файлы `will_be_deleted.txt` (с текстом `will_be_deleted`) и `will_be_moved.txt` (с текстом `will_be_moved`) и закоммите их с комментарием `Prepare to delete and move`.
1. В случае необходимости обратитесь к [официальной документации](https://git-scm.com/book/ru/v2/Основы-Git-Запись-изменений-в-репозиторий) — здесь подробно описано, как выполнить следующие шаги. 
1. Удалите файл `will_be_deleted.txt` с диска и из репозитория. 
1. Переименуйте (переместите) файл `will_be_moved.txt` на диске и в репозитории, чтобы он стал называться `has_been_moved.txt`.
1. Закоммитьте результат работы с комментарием `Moved and deleted`.

### Проверка изменения

1. В результате предыдущих шагов в репозитории должно быть как минимум пять коммитов (если вы сделали ещё промежуточные — нет проблем):
    * `Initial Commit` — созданный GitHub при инициализации репозитория. 
    * `First commit` — созданный после изменения файла `README.md`.
    * `Added gitignore` — после добавления `.gitignore`.
    * `Prepare to delete and move` — после добавления двух временных файлов.
    * `Moved and deleted` — после удаления и перемещения временных файлов. 
2. Проверьте это, используя комманду `git log`. Подробно о формате вывода этой команды мы поговорим на следующем занятии, но посмотреть, что она отображает, можно уже сейчас.

### Ответ

![image](https://github.com/user-attachments/assets/cdf1fb27-aaf9-4f4c-8081-448f4f931e4f)


### Отправка изменений в репозиторий

Выполните команду `git push`, если Git запросит логин и пароль — введите ваши логин и пароль от GitHub. 

В качестве результата отправьте ссылку на репозиторий. 

----

### Правила приёма домашнего задания

В личном кабинете отправлена ссылка на ваш репозиторий.


### Критерии оценки

Зачёт:

* выполнены все задания;
* ответы даны в развёрнутой форме;
* приложены соответствующие скриншоты и файлы проекта;
* в выполненных заданиях нет противоречий и нарушения логики.

На доработку:

* задание выполнено частично или не выполнено вообще;
* в логике выполнения заданий есть противоречия и существенные недостатки. 
