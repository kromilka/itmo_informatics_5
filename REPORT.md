# Отчет по Лабораторной №5
## Предварительные требования
1. Основы работы с Git (лабораторная работа по введению в Git).
2. Установленный Git на локальной машине.

## Введение
Данная лабораторная работа выполнялась на хостовой машине с ОС Windows, так как 3 виртулки были насмерть перегружены после запуска докеров на длительное время. (Восстанавлению не подлежали, а ноут не выдержит еще раз переустанавливать линукс самостоятельно, перегревается в жару, т.к. лабораторная выполнялась в дни, когда наступило +26 градусов на улице) 

Предварительно был создан новый публичный репозиторий с названием [git-practice](https://github.com/kromilka/git-practice) (рисунок 1).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/9d25ec2b-6b9d-48f3-bd2a-70e064c6b884)

Рисунок 1

Этот репозиторий был склонирован в папку по скопированному URL репозитория (рисунок 2).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/bc49b749-54be-45bc-8041-667d1af09d2b)

Рисунок 2

Далее необходимо было перейти в склонированный репозиторий и создать новый текстовый файл example.txt (рисунки 3-4).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/a4d551d9-1d7b-4cb9-9b9d-e3767d020a26)

Рисунок 3

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/6555c70d-0a38-4004-93e8-d18107f47ebd)

Рисунок 4

После этот файл согласно указаниям в Лабораторной работе был загружен в репозиторий на github с помощью слудеющих комманд:
```
git add example.txt
git commit -m "File added example.txt"
git push origin main
```
Так был добавлен файл example.txt (рисунок 5).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/c3ff10d3-8d92-4c35-aa72-767a72cd505d)

Рисунок 5

Далее была создана новая ветка `feature-branch` и необходимо было на нее переключиться (рисунки 6-7)

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/46c3ff00-8dc5-4cfc-8ed2-8a33cbce6a17)

Рисунок 6

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/7693a415-0b4c-4118-92ac-0e76096baa17)

Рисунок 7

Далее для примера был добавлен текст в файл example.txt (рисунок 8) и опять добавлен на ветку, но с новым именем коммита (рисунок 9).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/edec10e0-e954-4950-9eaa-b8466b72fece)

Рисунок 8

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/d9201032-8cde-412d-a70b-f723e4877dcc)

Рисунок 9

Затем необходимо было переключиться на ветку main снова и слить изменения из вети feature-branch в основную (рисунки 10-11).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/f46527f3-64cf-44a0-823e-6bc0266c4918)

Рисунок 10

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/33639de3-31f2-47f9-a8f2-dfdafd8c5e6c)

Рисунок 11

Проверяем, что изменения успешно слиты и отобразились на github (рисунок 12)

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/261b2556-080b-47c3-815f-a8e4a489e250)

Рисунок 12


## Работа с ветками

Изначально был создан новый текстовый файл, названный book.txt с структурой книги (рисунок 13)

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/59908568-fee0-485c-bf12-6bc10d304c3f)

Рисунок 13

Далее была создана ветка "feature-login" для разработки новой функциональности согласно указаниям Лабораторной работы (рисунок 14).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/a8a74353-8778-46e5-9915-62d088d8a8b3)

Рисунок 14

После этого были внесены изменения в файл (добавлена 3 глава книги, рисунок 15). 

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/62243da5-4ef5-4a25-9385-59669ceeb316)

Рисунок 15

И этот файл был переименован и добавлен как README.md в ветку feature-login (рисунки 16-17).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/93dd6554-db10-43e4-ba96-21546167562d)

Рисунок 16

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/37b521db-3aa9-43b2-8f1b-2f6095aa1478)

Рисунок 17

Проверка, что в feature-login был совершерн push (рисунок 18)

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/8144c940-a103-4330-b8a1-e070a601cc9c)

Рисунок 18


## Работа с удаленным репозиторием
Вначале нужно было переключиться на основную ветку - main и внести в ней изменения: добавить README.md, содержащий только 2 главы (рисунки 19-)

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/33eccbd4-c523-4c63-84bf-ac4af4ad17c3)

Рисунок 19 - Текстовый файл, добавляемый на ветку main

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/0aedb319-8331-46d9-86ea-b16b0b52cab1)

Рисунок 20 - Добавление файла


## Моделирование конфликта

Для моделирования конфликта при слиянии, необходимо, чтобы у нас в одном и том же месте файла на разных ветках был разный текст, поэтому мы переходим на ветку feature-login и изменяем файл, меняя 2 главу в README.md, как показано на рисунке 21. Затем коммитим и пушим изменения на ветку feature-login (рисунок 22)

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/4c3fb666-b7a2-4d8a-92cb-54c20d788fa5)

Рисунок 21

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/b8bdf112-2886-4c6c-8ab3-b105bbd1b337)

Рисунок 22


## Разрешение конфликтов

Возвращаемся на основную ветку main (рисунок 23) и сливаем изменения (рисунок 24).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/681393ef-b545-4edc-be95-ada2a01370e9)

Рисунок 23

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/339bf71d-591e-4226-ae33-057d494148f2)

Рисунок 24 - Возникновение конфликта

Вот как он выглядит в файле README.md (рисунок 25).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/9798aa7a-882b-49dc-95f1-28e049e1e865)

Рисунок 25

Изменяем файл, решая конфликт (рисунок 26).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/298e2ff5-0962-490a-a6be-95c5c7344139)

Рисунок 26

Коммитим разрешение конфликта на основную ветку с сообщением (рисунок 27).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/e271d48f-99f4-4496-ab5b-72a16119f295)

Рисунок 27


## Автоматизация проверки формата файлов при коммите

В данном разделе стоит задача автоматизировать проверку формата файлов при коммите с использованием Git Hooks. В нашем случае необходимо проверять, чтобы все .txt файлы в репозитории соответствовали определенному формату.

Был создан bash-скрипт check_format.sh, который выполняет проверку .txt файлов на соответсвие маске new*.txt (рисунок 28).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/dbe48946-2af5-4d7f-8a68-bd0b14962fc4)

Рисунок 28

Далее необходимо добавить скрипт в папку .git/hooks с названием pre-commit (работает перед коммитом, рисунок 29).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/90dc9f07-82d7-4d9f-b123-b76fc92dca14)

Рисунок 29

Был создан файл new_file.txt (рисунок 30) и после была проведена проверка работы скрипта при попытке коммита (рсунок 31).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/82e00fe8-0123-4004-b21a-86bef6a47daf)

Рисунок 30

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/3fb76242-4e9d-4299-a15f-175e5338c082)

Рисунок 31


## Использование Git Flow в проекте
В данном разделе задача состоит в том, чтобы интегрировать Git Flow в проект для управления циклом разработки, создания релизов и управления hotfixes. 

Проверка установлен ли git flow (рисунок 32). В целом, можно сказать, что при установке на Windows Git Bash Git Flow устанавливается в составе пакета.

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/1635ba83-aa18-41ad-a89a-0281312b7965)

Рисунок 32

Далее была выполнена инициализация Git Flow (рисунок 33).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/b1d68fff-d45a-4fe5-a260-36e496a017c1)

Рисунок 33

Согласно указаниям лабораторной работы была создана ветка для новой функциональности "task-management" (рисунок 34)

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/878f1260-804b-45d4-959e-e989ead5fc05)

Рисунок 34

Был создан файл task_manager.py с кодов изображенном на рисунке 35.
![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/7b0f5029-55d5-4341-ac0f-6d2d74c1e747)

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/f73aa210-0793-4869-aec7-14e2675c1cb2)

Рисунок 35

Коммитим его изменения и завершаем фичу и объединяем с основной веткой (рисунок 36).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/77070128-f1cd-45e9-85a5-ea8a644b7f9d)

Рисунок 36

Затем переключаемся на ветку develop (хотя мы и так на ней, так как Git Flow автоматически переключится на ветку develop и выполнит слияние после предыдущей команды). И начинаем релиз v1.0.0 (рисунок 37).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/39e501af-0c50-48be-a409-add5b4cd0f8d)

Рисунок 37

После этого вносим изменения, связанные с релизом. В нашем случае обновляем версию в файле version.txt, а затем коммитим (рисунок 38).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/9b25fb75-13a0-437c-90b3-5a9102a94e7a)

Рисунок 38

Завершаем релиз командой `git flow release finish v1.0.0` (рисунок 39).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/9e020155-9692-4c0b-b590-54de760f1fa7)

Рисунок 39

В процессе исполлзования критических ошибок **не было**, но ради интереса был создан hotfix (рисунок 40).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/86b2f314-1669-478c-97de-2f0d4d01dffe)

Рисунок 40

Затем было внесено "значительное изменение" (рисунок 41).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/13acfa98-2aa7-4631-8e0e-ecdf0f3f110b)

Рисунок 41

Был сделан коммит для исправления "ошибки" (рисунок 42)

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/a54e34eb-7eca-49f5-ab5e-eb4e7b36624e)

Рисунок 42

Был завершен hotfix (рисунок 43).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/d5995212-bdaa-4c42-9ca2-3f1efa5c715a)

Рисунок 43

Была завершена работа и отправлены все изменения на удаленный репозиторий (рисунок 44-45).

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/4e6febad-20be-4c27-95ef-45f72603e3d1)

Рисунок 44

![image](https://github.com/kromilka/itmo_informatics_5/assets/60718613/5e129e7c-dd9e-4d74-b898-e04fd3cc399a)

Рисунок 45

[Репозиторий](https://github.com/kromilka/git-practice)
