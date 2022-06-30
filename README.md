***Инструкция по работе с репозиторием***

**Решение задач из курса https://stepik.org/course/512/promo**

1. Зарегистрироваться на github.com
2. Скинуть свой логин
3. Склонировать проект 

    3.1 git clone https://github.com/Alllecs93/stepic_python.git
  
    или

    3.2 https://i.stack.imgur.com/XfKA5.png
  
4. Настроить git на ПК

    4.1 Set your username: git config --global user.name "FIRST_NAME LAST_NAME"

    4.2 Set your email address: git config --global user.email "MY_NAME@example.com"
5. Сгенерировать и добавить ssh-key https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

    5.1 Windows cmd (выполнить в командной строке):

    5.1.1 powershell

    5.1.2 ssh-keygen.exe -t ed25519 -C "MY_NAME@example.com"

    5.1.3 По желанию заполнить все поля (необязательно) и нажать Enter

    5.1.4 Сохранить указанный путь:  C:\Users\USERNAME/.ssh/id_ed25519.pub

    5.1.5 cat C:\Users\USERNAME/.ssh/id_ed25519.pub

    5.1.6 Скопировать строку ssh-ed25519 .....

    5.1.7 Зайти в профиль github по пути "Settings -> SSH and GPG keys" и нажать "New SSH key"

    5.1.8 В поле "Key" вставить строку из п. 5.1.6, заполнить название Title

    5.1.9 exit (для выхода из powershell)

    5.2 Или загуглить как сгенерировать ssh ключ и добавить в git

6. См. файл с инструкцией. В проекте создать свою ветку с названием автора и задачи (author/task_name), например "alexander/3.1_functions_1"

    6.1 Для этого в PyCharm нажать на название ветки, в списке веток нажать на master, далее выбрать "New Branch from Selected..." и ввести название ветки

    6.1.1 Либо выполнить git checkout -b branch_name, например "git branch -b alexander/3.1_functions_1"

    **6.2 Создать каталог с названием автора (ваше имя)**

    **6.3 Написать программу с комментариями и названием файла соответсвующим задаче в своем каталоге**

    6.4 Слева или через вкладку Git выбрать "Commit"

    **6.5 Ввести осмысленное описание выполненных работ**

    6.6 Выбрать файл и нажать "Commit"

    6.7 Для перезаписи коммита необходимо заранее нажать "Amend"

    6.8 По окончанию работ выполнить push (через зеленую стрелку вверх или вкладку Git -> Push)
7. Зайди на страницу проекта в github и создать pull request
8. Исправить замечания на code review
9. Ожидать merga в master
