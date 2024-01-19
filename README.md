**ПРЗ 4.2 Контроль целостности**

Выполнил
Студент 1 курса
Группы ББМО-01-23 
Белов Владимир Станиславович
Шифр 23Б1716

==========================================================================================
Задание
Astra Linux SE
1. Скачать и развернуть ВМ с ОС Astra Linux для отработки практических заданий
2. Включить мандатный контроль целостности (МКЦ) в соответствии с руководством по Wiki, КСЗ
3. Проверить работу механизма МКЦ (запрет на запись "вверх" - NWU), в отчете показать
блокировку доступа
4. Включить режим замкнутой программной среды (ЗПС), проверить работу механизма (попытка
запуска неподписанного исполняемого файла), в отчете показать блокировку доступа
5. Настроить и продемонстрировать работ утилит контроля целостности и регламентного
контроля целостности gostsum, afick
=======================================================================================
1) Для выполнения практики был скачан образ Astra Linux с файла практики (https://1drv.ms/u/s!Ap1Ijs338IQ9gZFmLJ5hn45FgcVLoQ?e=VcMkNU)
1.1) Установлена версия системы "Смоленск" с максимальным уровнем защиты

![image](https://github.com/V0vochka/Praktika-4/assets/70959108/2bfbb911-5e49-434a-9ed9-8d57e8dec769)

Произведена настройка мандатного управления доступом

![image](https://github.com/V0vochka/Praktika-4/assets/70959108/ff192f9c-13f3-4595-835a-f9af7891e363)

Для измнения конфигурации мандатного контроля целостности в Astra Linux необходимо запустить утилиту "политика безопасности"

![image](https://github.com/V0vochka/Praktika-4/assets/70959108/62a27f1c-feb9-46ee-8d84-4e64d5a34eae)

В меню "Режим эксперта" назначаем уровни целостности для директорий "Документы" и "Изображение". 

![image](https://github.com/V0vochka/Praktika-4/assets/70959108/1e811549-a2f7-4708-aef0-bf762d192c46)

Проверим уровни контроля

![image](https://github.com/V0vochka/Praktika-4/assets/70959108/3fc02bd8-1635-4b8a-b654-6640a08e9fd4)

Копирование файла с атрибутом ниже в папку с атрибутом выше не сработало - была получена ошибка доступа. В то же время "запись вниз" работает.

Режим замкнутой программной среды (ЗПС)

![image](https://github.com/V0vochka/Praktika-4/assets/70959108/4ea8619d-8384-4d01-a108-fa978f6a2242)

В качестве тестового файла был взят установщик телеграма

![image](https://github.com/V0vochka/Praktika-4/assets/70959108/85c8debd-5f47-4591-b081-ab508890da30)

![image](https://github.com/V0vochka/Praktika-4/assets/70959108/ce9f3009-2849-49e2-bf87-e33efb7966dc)

