# Это репозиторий для обучения pull request

## Первые шаги

1. Делаем fork репозитория, в которой потом хотим сделать pull request. Ищем кнопку Fork на странице репозитория <https://git@github.com:gulden-geekbrains/version_control.git>
2. Выполняем команду клонирования из своей fork-копии
```sh
git clone git@github.com:*YOURE_GITHUB*/version_control.git
```
3. Создаем новую ветку и вносим необходимые изменения в файл
```sh
git checkout -b updatereadme
vim README.md
git add README.md
git commit -m "Добавили инструкцию как создать pull request"
```
4. Делаем push  
```sh
git push --set-upstream origin updatereadme
```
5. Переходим на свою страницу репозитория. Выбираем ветку **updatereadme** и жмем кнопку **Compare & pull request**

## Заметки

Что бы сделать push от другого пользователя необходимо выполнить команду
```sh
GIT_SSH_COMMAND='ssh -i ~/.ssh/user-private-key -o IdentitiesOnly=yes' git push git@github.com:gulden-geekbrains/version_control.git
```

вместо *user-private-key* подставьте свой ключ

Можно прописать настройки для подсоединения по ssh
```sh
git config remote.origin.url git@github.com:gitusername/reponame
git config core.sshCommand "ssh -i ~/.ssh/user-private-key -o IdentitiesOnly=yes"
```
# Как подружить git с github под Windows 10

Вот видео инструкция https://youtu.be/E8cIjbJMEpE


# инструкция домашняя работа

## работа с текстом
здесь у меня конфликт с веткой текст_текст

чтобы сделать курсивов поставить (*) по сторонам текста. *Пример курсив*

чтобы сделать полужирным (**) **например полужирный**

***полужирный курсив***

зачеркнутое (~~)~~ТЕКСТ~~

### работа со списком
* без нумерации списка
* перед текстом
* ставим (*)
+ 4

1. с нумерацией 
2. перед текстом
3. пример (1.; 2.; n. ...) 
+ 4
#### заголовок 3
виды текста через нижний пробел (_)

 жирный __текст__  

 другой курсив  _текст_ 

 и еще образ жирного курсива ___текста___

##### заголовок 4
![foto-moto](foto-moto.jpg)

думаю на этом все
###### заголовок 5
это конец 
 # FINISH !
 
делаем форк c той репозитории нак которой хотим по работать

потом скачиваем к себе git clone :\hhtps..... 

создаем ветку git branch "имя ветки" 

вносим дополнения  git add "имя файла" 

 потом фиксируем наши допалнения git commit -m "text"

 дальше проверить через git status

git push -u origin main команда для заливки в облако полную репозиторию

git push --set-upstream origin intruction залить в облако ветку репозиторию

git pull забираем с облака 
