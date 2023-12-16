# Отчет по лабораторной работе №5
## Введение
1. Сначала я создал репозиторий _git-practice_ на _GitHub_ и скопировал его _URL_-адрес. Далее с помощью терминала и команд _git clone_ и _cd_ я перешел в папку для локального сохранения репозитория.
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/accd2ce2-5b31-40b8-8dc1-99fc7daa9330)
3. Потом я создал новый текстовый файл _test.txt_, добавил в него некоторый текст и запушил на _GitHub_ в основуную ветку, используя команды _git add_, _git commit -m_ и _git push_.
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/1ffc178d-2b25-496a-8e4b-27951a7e579a)
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/6370c231-c393-42a7-8904-2c68f8908a35)
5. Затем я создал новую ветку _feature_ с помощью команды _git branch_, переключился на нее с помощью _git checkout_.Я отредактировала файл, повторил некоторые шаги из пункта 3, переключился обратно в основную ветку с помощью _git checkout main_ и слил изменения из _feature_ в основную ветку, используя _git merge_ и _git push_.
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/83cd7154-317d-4a05-b9ff-5a2fc2d92936)
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/ba38b7c8-8fa5-482f-aea2-b71ed52b9071)

Изменения успешно слиты и отображаются в основной ветке на GitHub. 
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/908141be-aa70-4e23-b614-0b1a2cd8479c)

## Работа с ветками
1. Я создал новый текстовый файл с базовой структурой книги _book_. И запушил в отдельном коммите.
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/a4ab3e35-d09a-4c72-bff3-98f83d627bba)
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/fb6818c5-8399-42e0-9293-81e638a41320)

2. С помощью _git checkout -b_ создал новую ветку _feature-login_.
3. Далее я внес изменения в файл, закоммитил их и отправил ветку на _GitHub_, используя _git add_, _git commit -m_, _git push origin_.
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/3c0b8deb-d67a-4c78-a384-8016babbfa2c)
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/863b46ba-fcea-43ea-a54f-79d0498abb0e)

## Работа с удаленным репозиторием
1. Я переключился на основную ветку, внес изменения в файл _book_, закоммитил изменения и отправил их на _GitHub_ с помощью _git add_, _git commit -m_, _git push origin_.
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/3bcd1767-f22b-4450-9327-a609dc9a5b4c)
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/16c22183-f8e9-4210-85fb-0da6fc29a72a)

## Моделирование конфликта
1. Я вернулся в ветку _feature-login_, изменил главу 2 в файле _book.txt_, закоммитил изменения и отправил их на _GitHub_
2. ![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/3224fded-51bc-41d5-acd0-a0c06626c1fb)
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/1386d363-586b-4cd2-a1d9-f0ff348ae2d7)

## Разрешение конфликта
1. Я вернулся в основную ветку и попробовал слить изменения с помощью _git checkout main_ и _git pull origin main_. Возник конфликт.
2. Я разрешил конфликт, удалив метки и оставив нужные изменения.
3. Я закоммитил решение конфликта и отправил его на _GitHub_.

## Автоматизация проверки формата файлов при коммите



