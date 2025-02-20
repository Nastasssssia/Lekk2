# Привет! Меня зовут Git и я система контроля версий. Я отслеживаю и веду историю изменения в файле и помогаю управлять им. 
## Сейчас я раскажу немного о том что я умею:

1. создавать и хранить множество вариантов написанной версии файла (кода), изучать его изменения и тденфицировать ошибки;

2. объединять код разных людей в одновременной работе, объединять изменения;

3. создавать и управлять ветками, что позволяет более безопасно изменять код;

4. автоматически создавать резервные копии кода;

5. сравнивать историю разных версий файла, для быстрого доступа ко всем изменениям.

**Сейчас я помогу тебе научиться работать с моими функциями, следуй за мной.**

* Видимо, ты уже установил меня на свой компьютер, скачав меня с официального сайта https://git-scm.com/downloads, так же не забудь скачать и VS Code, без него я не работаю; 

* Мы запустли с тобой меня. Теперь создай на удобном для тебя диске, папку где мы будем с тобой работать. В VS Code, через Open file найди папку и открой ее. Все, в левой части ты видишь папку которую выбрал, теперь в ней надо создать файл. Для этого, там же нажи New file - дай ему имя и не забуть о расширении. У меня сейчас стоит имя с расширением .md;

* Теперь открываем терминал, он находиться в View - terminal. В низу у нас открылась консольная панель. Теперь мы можем начать работать в ней. 

Сейчас давай познакомися с тобой, для этого в терминале набери следующие команды:

**git config --global user.name "твое имя"**

**git config --global user.email "твой email"**

*Это нужно для того, что бы я знал, ко вносит изменения в файл.*

**Теперь изучим мои команды, что бы я мог работать и помогать тебе.**

Все команды ты вносишь в терминал. Если после ввода команды, я как то странно ругаюсь на тебя, в моем тексте всегда есть подсказка, что происходит, почему я не выполняюю ту или иную команду, иногда я не ругаюсь а говорю, что выполнил то или иное действие. Иногда и ты можешь сделать ошибку и дать не ту команду, будь внимателен. А, теперь поехали (да, чуть не забыл, установи сразу автосохрание за своим файлом что бы каждый раз не следить за сохрением, File - Avto Save):

* создаем свой первый репозиторий в своей папке с помощью команды git init;

* теперь давай проверим установлен лия я правильно и какая версия стоит, для этого введем команду git  --version (не забываем о пробеле перед --), если все хорошо, то высветиться git version 2.41.0 а возможно и другая;

* теперь ты можень начать писать все что тебе нужно над терминалом, ты сделал это, отлично, теперь давай проврим мой статус, для этого дай команду git status (ты увидишь что я тебе отвечу

On branch master

Changes not staged for commit:

  (use "git add <file>..." to update what will be committed)

  (use "git restore <file>..." to discard changes in working directory)
        modified:   Git_homework.md)

        все хорошо, это значит у меня есть не отслеживаемые изменения.
* выше я дал тебе подсказку что делать дальше, требуеться сохранить изменения, теперь введи команду git add и имя файла как ты меня назвал;

* все, ты сохранил мения, теперь давай дадим имя моему изменения следующей командой git commit -m "Работа с командами 2" - любой текст который тебе нужен.

Отлично ты видишь - [master 36d3a6a] Работа с командами 2

 1 file changed, 15 insertions(+) - это значит что я сохранил твои изменения с пометками.
 
 * так же у меня есть хорошая команда, когда ты можешь узнать о статусе своего файла введя команду git status.

 **Введя команду git log - ты увидешь все измения что внес в файл с указаниями коментариев которые ты делал. (кстати если на этой команде у тебя завис терминал, просто нажми Q).**
* что бы понять есть ли отличи в файлах введи команду git diff (и ты увидишь ответ, есть ли изменения или нет, если же от мення не последует ответа то это значит что текущее состояние файла и состояние согхраненого файла ничем не отличаеться).
* если ты хочешь походить по разным версиям сохраниения файла, то введи команду git checkout и введем первые четыре цифры сохраненого нами файла (он выделен желтым цветом и выглядит вот так - commit 36d3a6a7b06366fe7558d02f0c9ae6e6caefa7ae), потом нажимаешь Tad, и я самм подтяну нужный нам номер и перейду в нужние для тебя сохранение файла.

# Работа с текстом
**Текст который ты пишешь над терминалом можно изменять языком Markdown"-это разметка текста. Есть определенные правила, я раскажу о некоторых:**
- если я пишу *что-то* вот так между звездочками, то текст будет курсивным;

* если я пишу **что-то** обрамляя текст по две звездочки с двух сторон, то текст будет жирным;

* заголовок пишеться через [##] перед текстом.

Что бы увидеть то как пишеться текст, то с правой стороны есть значек два прямоугольнка с лупой, нажав на них ты увидишь с правой стороны открывшееся окно где тыкст который ты пишешь тут, отрожаеться там, только он уже отличается от так как ты применяешь навыки языка Markdown.

Так же не забывай следить за веткой, в которой ты находишься, это указано в левом нижнем углу (у меня эта ветка master).

Если возле имени файла ты видишь какие либо обозначения:
- допустим то точка, то твой файл не сохранен;
* если буква М то я отслеживаю твой файл.


**Не забывай производить сохранения в файле, всегда читай мои подсказки в терминале, всегда проверяй команды которые ты пишешь и не пугайся, у тебя всегда есть самая главная команда git status.**

Так же могу порекомендовать к ознакомлению книгу по Git - https://git-scm.com/book/ru/v2

## Работа с ветками
* Мы можем создовать необходимое нам для работы колличество нужных нам веток. Наша основная ветка *master* это наш чистовик для работы.
## Для того что бы создать ветку требуеться в теминале требуеться ввести следующие команды:

 - - git branch (имя новой ветки) - у меня это выглядело (git branch bran);
 - - для перехода на нужную на ветку, для начало надо ввести git status (для проверки, что же у нас происходит в ветке). 
 - - - ввести git branch - для того что бы проврить на какой мы ветке. Если нас все устраивает - вводим команду git checkout (название нужной нам ветки).
 - - что бы убедиться что мы в нужной ветке - вводим git branch (и смотрим где мы находимся).
 - - вносим все изменения что нам надо, и действуем по обячной схеме (git status, git add, git commit -m)/

## Слияние веток - если нас устраивает все в нашй ветке, ее можно слить с нашим честовиком *master*, для этого 
- - переходим в основную ветку (git checkout master)
- - проверяем все ли гово для слияния (git status), если нас все устраивает то вводим - git merg (указываем нужную нам ветку), и если все сделано павильно то нужные нам втки сольються.
## Удаление веток
 Для корректного удаления нужно помнить несколько правил, чтобы не получить ошибки:

Нельзя удалить ветку, в которой вы находитесь. Git выкинет ошибку и не произведет удаление данной ветки. По этому нам нужно перейти на другую ветку.
Git не позволит удалить ветку, у которой есть несохраненные изменения. 
Для принудительного удаления ветки используется флаг -D с заглавной буквой. В этом случае ветка будет удалена независимо от текущего статуса, без предупреждений.

В обычном варианте используем git branch -d (имя ветки), если слияние прошло успешно и ветка нам не требуеться. 

## Конфликт при слиянии веток
* если у нас в ветках указан разный текст, то при слиянии у нас может возникнуть конфликт. 
* при слиянии такого случая, в основной ветке gut  предложит нам самому выбрать нужный нам вариант сохранения веток, их может быть несколько 
- - принять текущую версию
- - принять версию что пришла из другой ветки
- - принять оба варианта 

![Слияние](conflict.png)

## *Мы выбираем то что нам требуеться*


## Работа с изображениями

* В большинстве проектов есть файлы или целые директории, в которые мы не хотим (и, скорее всего, не захотим) коммитить. Мы можем удостовериться, что они случайно не попадут в git add -A при помощи файла .gitignore

- Создаь вручную файл под названием .gitignore (только так и никак иначе!!!) и сохраняем его в директорию.
- Внутри файла перечислим названия файлов/папок, которые нужно игнорировать, каждый с новой строки (второй вариант можно указать *.png  *таким образом все файлы с расширением png, будут игнорироваться).
- Файл .gitignore должен быть добавлен, закоммичен.

 **Вариант указания как правильно прописываеться картинка.**
![Картинка](Logo.png)

## Визуализация веток, для этого понадобиться следующая команда: 
- git log --graph


Спасибо за внимание, до скорой встречи))))