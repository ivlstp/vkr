# Блокировка доступа к несанкционированным сетевым папкам в локальной сети

## Описание защитной меры
### Цель:
+ сокращение каналов утечки информации
+ уменьшение возможностей для горизонтального перемещения в локальной сети;
+ снизить возможность загрузки ВПО с несанкционированной общей сетевой папки SMB;
+ противодействие атакам на перехват сессии и кражу паролей (SCF File Attacks).

На уровне источника (ПК и серверы) нужно ограничить исходящие соединения к сетевым папкам (SMB shared folder), оставив доступ только к списку легитимных сетевых папок.
Варианты реализации:

+ Локальный межсетевой экран
+ DLP с функцией контроля SMB протокола, например КИБ SearchInform

Общий алгоритм действий

1. Определить перечень легальных SMB шар и узлов, к которым необходимо подключаться по SMB
2. Настроить белый список на локальных СЗИ
3. Включить блокировку 

Важно: SMB один из ключевых протоколов для локального взаимодействия в доменной инфраструктуре. Перед включением блокировки необходимо провести тщательный аудит всех информационных потоков по протоколу SMB.

### *Рекомендации к заполнению карточки*:
+ Описать в карточке общую политику в отношении сетевых файловых ресурсов,
+ Средство защиты, которым осуществляется блокировка, присоединить к карточке как Инструмент,
+ Добавить Инструкцию (например, в заметках к мере) по добавлению/исключению каталогов из доступа 
+ Если ведется учет (реестр) сетевых файловых ресурсов - вести его в разделе Объекты файловой системы \ Файлы и папки 
+ Создать шаблон регулярной задачи на актуализацию списка общих сетевых папок и прав.

## Связанные угрозы и уязвимости
|Угроза|
|-|
|[Раскрытие ключей (паролей) доступа](/vkr/threats/page2)|