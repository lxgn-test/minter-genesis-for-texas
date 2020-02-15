# minter-genesis-for-texas

## 1. Создание genesis.json с помощью Exporter Tool

Инструкция по созданию genesis файла по этой ссылке (https://gist.github.com/danil-lashin/99618f9ac245444d3ecf5362f2f6d5d2) 

## 2. Входные данные:

В файле genesis.json находиться файл снимка сети на определенный блок, созданный в предыдущем пункте

В файле changes.txt находятся данные с со списка валидаторов (https://docs.google.com/document/d/1rOpGUEi1u1T4OeWhpBZn_Wguince8lk-TVUSiCmT3ME/edit?usp=sharing)

## 3. Команда для запуска

```bash
php changer.php
```
или
```bash
./changer.php
```

## 4. Результат

Измененный файл в формате genesis.YYYY-MM-DD-HH-MM-SS.json

Пример - genesis.2020-02-15-20-14-15.json

## 5. Как работает

Для исключения дубликатов - обратабатывается файл валидаторов, меняются адреса с маиннета, на указанные для тестнета, и наоборот.
