# *Git* — это система для управления версиями исходного кода программ. Она позволяет отслеживать любые изменения в файлах, хранить их версии и оперативно возвращаться в любое сохранённое состояние.

# **Зачем нужен Git**:

Позволяет разработчикам параллельно работать над проектом. Это помогает не мешать друг другу и добавлять в основную версию только качественный код. 
Обеспечивает полный контроль над каждым вариантом продукта. В любой момент можно вернуться в прошлое и восстановить предыдущую версию программы, если новый релиз всё поломал. 
Помогает «откатывать» любые изменения. В разработке часто меняются требования к проекту, видение заказчика и стандарты дизайна. Полный контроль над всеми итерациями приложения позволяет легко «откатывать» любые изменения и вносить поверх них новые.

# Установка Git и Visual Studio Code

➤Установка Git для Windows, MAC, Linux: https://git-scm.com/downloads

➤Установка VSCode для Windows, MAC, Linux: https://code.visualstudio.com/Download

При первом использовании Git необходимо представиться. Для
этого нужно ввести в терминале 2 команды:

git config --global user.name «Ваше имя английскими буквами» git

config --global user.email ваша почта@example.com

# Основные команды Git
## Введение в контроль версий. Работа с Git. Составление инструкции по работе с Git.
✦ git init – инициализация локального репозитория 
## Подготовка репозитория
* Создать папку в необходимом репозитории компьютера
* Перейти с помощью проводника в **Visual Studio Code** в созданную папку
* Инициализировать репозиторий в терминале командой ```git init```
* 
![Изображение](https://github.com/Genius1107/Readme/blob/main/Screenshots/1%20(1).png)


✦ git status – получить информацию от git о его текущем состоянии

![Изображение](https://github.com/Genius1107/Readme/blob/main/Screenshots/5404576886266392974.jpg)

✦ git add – добавить файл или файлы к следующему коммит

Для добавление изменений в коммит используется команда ```git add``` и имя файла<br>
Например, ```git add README.md```

![Picture](https://github.com/Genius1107/Readme/blob/main/Screenshots/git%20add.jpg)


✦ git commit -m “message” – создание коммита.
```git commit -m "first commit"``` - команда для отправки коммита<br>
* ```git commit``` - обращение к **GIT**
* ```-m``` - добавить сообщение *(коментарий)*
* ```"first commit"``` - коментрарий *(в кавычках)*
## Как писать сообщения для коммитов
Старайтесь писать комментарии по-английски — это считается хорошим тоном. Но Git
понимает кириллицу, и писать комментарии на русском можно, например, в том случае,
если вы на 100% уверены, что ваш код будет интересен только русскоязычной аудитории
Общие правила написания сообщений
для коммитов:
1. Пишите сообщения с заглавной буквы
2. Не используйте прошедшее время
3. По возможности указывайте на исходный код в сообщении
4. Пишите осмысленные сообщения (При написании сообщений для коммитов можно пользоваться формулой:
«Что сделать + для какой сущности + подробности (необязательно)».)

Команда, которая позволяет оставить сообщение для коммита:

![picture](https://github.com/Genius1107/Readme/blob/main/Screenshots/gitvommit.jpg)

✦ git log – вывод на экран истории всех коммитов с их хеш-кодами
```git log``` - стандартный вид
* ```git log --graph``` - вид с графическим отображением веток

![picture](https://github.com/Genius1107/Readme/blob/main/Screenshots/git%20log.jpg)
 
✦ git checkout – переход от одного коммита к другому
 ```git checkout```
* ```git checkout <номер коммита, первые 4 символа>``` - перейти к определенному изменению
* ```git master``` - перейти к изменению последнего коммита
✦ git checkout master – вернуться к актуальному состоянию и продолжить работу

![picture](https://github.com/Genius1107/Readme/blob/main/Screenshots/git%20checout.jpg)

Введение в контроль версий. Работа с Git. Составление инструкции по работе с Git.

# **Справочник по Markdown от Microsoft:**
https://docs.microsoft.com/ru-ru/contribute/markdown-reference

✦ # Заголовок – выделение заголовков. Количество символов “#” задаёт уровень заголовка
(поддерживается 6 уровней).

✦ = или - – подчёркиванием этими символами (не менее 3 подряд) выделяют заголовки первого
(“=”) и второго (“-”) уровней.

✦ ** Полужирное начертание** или __ Полужирное начертание__

✦ *Курсивное начертание* или _Курсивное начертание_

✦ ***Полужирное курсивное начертание***

✦ ~~Зачёркнутый текст~~

✦ * Строка – ненумерованные списки, символ “*” в начале строки

✦ 1, 2, 3 … – нумерованные списки

## Работа с ветками
* ```git branch``` - посмотреть список веток
  
![picture](https://github.com/Genius1107/Readme/blob/main/Screenshots/git%20branch.jpg)
  
* ```git branch <название ветки>``` - создать ветку (новая ветка унаследует коммиты родительской ветки)
  
![picture](https://github.com/Genius1107/Readme/blob/main/Screenshots/image%20(2).png)
  
* ```git checkout <название ветки>``` - перейти на ветку
  
![picture](https://github.com/Genius1107/Readme/blob/main/Screenshots/git%20checout.jpg)
  
* ```git branch -d <название ветки>``` - удалить ветку после merge
* ```git branch -D <название ветки>``` - удалить ветку принудительно
  
![picture](https://github.com/Genius1107/Readme/blob/main/Screenshots/git%20branch%20-D.jpg)
  
* ```git merge <название сливаемой ветки>``` - сливание веток
  
![picture](https://github.com/Genius1107/Readme/blob/main/Screenshots/git%20merge.jpg)
  
* При слияние веток(если в обеих ветках были изменения) могут возникнуть ошибки слияния, где гит предложит самостоятельно редактировать текст:
  
![](https://github.com/Genius1107/Readme/blob/main/Screenshots/%D0%BE%D1%88%D0%B8%D0%B1%D0%BA%D0%B0.jpg)
  
# Настройка SSH для GitHub

***SSH*** (англ. Secure SHell — безопасная оболочка) — это сетевой протокол для зашифрованного
соединения между клиентом и сервером; по этому протоколу можно безопасно передавать
данные.

При подключении по SSH применяют пары криптографических ключей: открытый (public,
публичный) и закрытый (private, приватный). Пользователь создаёт ключи специальной командой
в терминале и сохраняет закрытый ключ на своём компьютере. Открытый ключ сохраняется на
сервере, например, в настройках аккаунта на GitHub.

При соединении с сервером проверяется соответствие этих ключей друг другу, и если проверка
пройдена успешно — пользователю разрешается доступ на сервер.

При аутентификации по ключу закрытая часть (private key) всегда передаётся в зашифрованном
виде. Закрытый ключ можно защитить паролем. При соединении клиент запросит этот пароль
перед тем, как сравнить ключи.

Создание SSH-ключей
Запустите Git Bash или Терминал VSC (если у вас Windows) или Терминал (на Linux/MacOS).
Выполните команду ssh-keygen:

![](https://github.com/Genius1107/Readme/blob/main/Screenshots/ssh%20keygen.jpg)

Консоль попросит ввести путь к файлу, в который будут сохранены сгенерированные ключи, и
одновременно предложит сохранить их в файл по умолчанию:
Enter file in which to save the key (/home/имя_пользователя/.ssh/id_rsa): 

![](https://github.com/Genius1107/Readme/blob/main/Screenshots/%D0%B8%D0%B7%D0%BE%D0%B1%D1%80%D0%B0%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5_2025-03-23_214419070.png)

Сохраните ключи в папку по умолчанию: для этого нажмите Enter на Windows или Return на
macOS. В уроках мы исходим из того, что ключи сохранены именно в дефолтной директории.
При создании ключей система попросит придумать пароль для доступа к ключам. Когда вы будете
задавать пароль, в терминале ничего не отобразится, даже звёздочки:
Enter passphrase (empty for no passphrase): 

![](https://github.com/Genius1107/Readme/blob/main/Screenshots/%D0%B8%D0%B7%D0%BE%D0%B1%D1%80%D0%B0%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5_2025-03-23_214546172.png)

Обязательно создайте пароль и запомните его — это дополнительная мера безопасности на тот
случай, если ваш приватный ключ попадёт не в те руки.
Рисунок в окне терминала будет свидетельствовать, что ключи успешно созданы:

![](https://github.com/Genius1107/Readme/blob/main/Screenshots/%D0%B8%D0%B7%D0%BE%D0%B1%D1%80%D0%B0%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5_2025-03-23_214812754.png)

Теперь необходимо сохранить открытый ключ в вашем аккаунте на GitHub.
Выведите ключ в терминал командой:
cat .ssh/id_rsa.pub
Скопируйте ключ от символов ssh-rsa , включительно, и до конца:

![](https://github.com/Genius1107/Readme/blob/main/Screenshots/%D0%B8%D0%B7%D0%BE%D0%B1%D1%80%D0%B0%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5_2025-03-23_215237021.png)

Зайдите в свой аккаунт на GitHub, перейдите в раздел настроек:

![](https://github.com/Genius1107/Readme/blob/main/Screenshots/%D0%B8%D0%B7%D0%BE%D0%B1%D1%80%D0%B0%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5_2025-03-23_215543613.png)

Выберите пункт SSH and GPG keys; для создания нового ключа нажмите на кнопку New SSH key в
правом верхнему углу:

![](https://github.com/Genius1107/Readme/blob/main/Screenshots/%D0%B8%D0%B7%D0%BE%D0%B1%D1%80%D0%B0%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5_2025-03-23_215759661.png)

Откроется страница с двумя полями ввода:
• Title (заголовок ключа). Когда будете задавать заголовок, учитывайте, что в дальнейшем
вы, возможно, добавите и другие ключи. Например, с другого своего компьютера, чтобы
получить с него доступ к репозиториям на GitHub. Поэтому выбирайте для каждого ключа
уникальные заголовки, например ключ с домашнего компьютера можно назвать HomePC,
а с рабочего — WorkPC.
• Key (ключ). Сюда необходимо вставить скопированный из терминала ключ.

![](https://github.com/Genius1107/Readme/blob/main/Screenshots/%D0%B8%D0%B7%D0%BE%D0%B1%D1%80%D0%B0%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5_2025-03-23_215958770.png)

Нажмите кнопку Add SSH key — ключ добавится к вашему аккаунту. Если вы захотите получить SSHдоступ к своему аккаунту на GitHub с нескольких компьютеров, для каждого из них должен быть
создан и добавлен свой SSH-ключ.

![](https://github.com/Genius1107/Readme/blob/main/Screenshots/%D0%B8%D0%B7%D0%BE%D0%B1%D1%80%D0%B0%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5_2025-03-23_220115754.png)


