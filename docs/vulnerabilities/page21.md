# Возможность открытия зараженных, вредоносных файлов

## Описание уязвимости
Пользователи могут открыть файл, который приведет к выполнению вредоносного кода. Злоумышленники могут использовать несколько типов файлов, которые требуют от пользователя их выполнения, включая .doc,. pdf,. xls,. rtf,. scr,. exe,. lnk,. pif и .cpl.
Злоумышленники  могут использовать различные формы маскировки файла, чтобы увеличить вероятность того, что пользователь откроет его.
Хотя ВПО часто используется для первоначального доступа, он может быть использован и на других этапах вторжения, например, когда противник помещает файл в общий каталог или на рабочий стол пользователя в надежде, что пользователь нажмет на него.
## Вхождение в базы ФСТЭК, MITRE ATT&CK
### Техники MITRE ATT&CK:
+ [T1204.002 User Execution: Malicious File](https://attack.mitre.org/techniques/T1204/002/)

## Связанные угрозы и меры защиты
|Угроза|
|-|
|[Заражение вредоносным программным обеспечением](/vkr/threats/page20)|

|Меры защиты|
|--------|
|[Контроль целостности файла hosts](/vkr/measures/page4)|
|[Централизация системы антивирусной защиты (АВЗ)](/vkr/measures/page6)|
|[Антивирусная защита рабочих станций](/vkr/measures/page16)|
|[Настройка безопасных заголовков для web сайта](/vkr/measures/page34)|
|[Проведение рассылки по информационной безопасности](/vkr/measures/page35)|
