# Отчет по лабораторной работе №5
## Введение
1. Я создал репозиторий _git-practice_  и отклонил его к себе.
   
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/accd2ce2-5b31-40b8-8dc1-99fc7daa9330)

2. Потом я создал новый текстовый файл _test.txt_, добавил в него некоторый текст и запушил в основуную ветку, используя команды _git add_, _git commit -m_ и _git push_.
   
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/1ffc178d-2b25-496a-8e4b-27951a7e579a)
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/6370c231-c393-42a7-8904-2c68f8908a35)

3. Затем я создал новую ветку _feature_ с помощью команды _git branch_, переключился на нее с помощью _git checkout_.Я отредактировал файл, повторил некоторые шаги из пункта 3, переключился обратно в основную ветку и слил изменения из _feature_ в основную ветку, используя _git merge_ и _git push_.
   
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/83cd7154-317d-4a05-b9ff-5a2fc2d92936)

![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/ba38b7c8-8fa5-482f-aea2-b71ed52b9071)

Изменения успешно слиты и отображаются в основной ветке на GitHub. 

![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/908141be-aa70-4e23-b614-0b1a2cd8479c)

## Работа с ветками
1. Я создал новый текстовый файл с базовой структурой книги _book_. И запушил в отдельном коммите.
   
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/a4ab3e35-d09a-4c72-bff3-98f83d627bba)

![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/fb6818c5-8399-42e0-9293-81e638a41320)

2. С помощью _git checkout -b_ создал новую ветку _feature-login_.
3. Далее я внес изменения в файл, закоммитил их и отправил ветку на _GitHub_.
   
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/3c0b8deb-d67a-4c78-a384-8016babbfa2c)

![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/863b46ba-fcea-43ea-a54f-79d0498abb0e)

## Работа с удаленным репозиторием
1. Я переключился на основную ветку, внес изменения в файл _book_, закоммитил изменения и отправил их на _GitHub_.
   
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/3bcd1767-f22b-4450-9327-a609dc9a5b4c)

![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/16c22183-f8e9-4210-85fb-0da6fc29a72a)

## Моделирование конфликта
1. Я вернулся в ветку _feature-login_, изменил главу 2 в файле _book.txt_, закоммитил изменения и запушил в удаленный репозиторий.
   
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/3224fded-51bc-41d5-acd0-a0c06626c1fb)

![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/1386d363-586b-4cd2-a1d9-f0ff348ae2d7)

## Разрешение конфликта
1. Я вернулся в основную ветку и попробовал слить изменения с помощью _git checkout main_ и _git pull origin main_. Возник конфликт.
2. Я разрешил конфликт, удалив метки и оставив нужные изменения.
3. Я закоммитил решение конфликта и отправил его на _GitHub_.

## Автоматизация проверки формата файлов при коммите
1. Я создал _bash-script_, который будет выполнять проверку формата .txt файлов на наличие символа.
   
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/1472ddef-bfb5-4e8a-98f2-5385d38678a7)

2. Я добавил скрипт в репозиторий, поместив его в папку _.git/hooks_ и убедившись, что у него есть права на выполнение с помощью _cp_ и _chmod +x_.
```
cp check_format.sh .git/hooks/pre-commit
chmod +x .git/hooks/pre-commit
```
3. Далее я попробовал внести изменения и закоммитить. Теперь, при каждой попытке закоммитить изменения, Git будет автоматически выполнять проверку формата файлов перед коммитом.
4. При возникновении необходимости внести изменения в файлы, чтобы они соответствовали формату, нужно внести изменения, добавить файлы и снова попробовать закоммитить.

## Использование Git Flow в проекте
1. Установил git-flow
2. Инициализировал Git Flow
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/9a55da27-695b-42fa-af2b-0a0c3ba69f60)

4. Создал ветку для новой функциональности "tesk-management" и создал новый файл task_manager.py:
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/87015b84-9a5a-4754-906e-44c5e816e708)

6. Закоммитил, завершил фичу и объединил ее с основной веткой:
  ```
  git flow feature finish task-management
  ```
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/56744741-e892-485c-ad9d-8c0a0f63e358)

Git Flow автоматически переключился на ветку develop и выполнил слияние. Конфликтов не было.
5. Создал новый релиз 
``` 
git flow release start v1.0.0
```
Внес изменения, закоммитил и завершил релиз.
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/6926f5e7-621e-4b3b-bd46-19a3ffa02fbb)

![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/ed54623e-ee1a-40dc-9e4d-056e9baf91b8)

6. Пусть у нас выявлена критическая ошибка, создаем hotfix:
```
git flow hotfix start hotfix-1.0.1
```
Вносим изменения для исправления ошибки и коммитим.
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/3ddf9a8d-2e94-4ca5-b531-e49e73f9d843)

После завершаем hotfix и объединяем его с ветками develop и main.
![image](https://github.com/Andrzakourcev/git-practice/assets/144477949/98d81ce9-8bb2-49fd-b442-b07ca1e41cd2)

7. Пушим все в удаленный репозиторий.
