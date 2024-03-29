# Межсетевое экранирование на границе сети

## Описание защитной меры
### Цель: защита ключевых активов от несанкционированного доступа на сетевом уровне. 

Установка и настройка межсетевых экранов на все точки входа/выхода между локальной сетью и Интернет или между сетевыми сегментами.
Реализуются базовые функции экранирования:

+ фильтрация трафика на уровне интерфейсов, IP адресов и портов (L2-L4);
+ трансляция адресов (NAT);
+ регистрация событий.

### *Рекомендации к заполнению карточки:*
+ Описать базовую политику межсетевого экранирования, включая ACL;
+ Дополнительные инструменты анализа сетевого трафика (ids/ips, url filtering, application filtering и т.д.) могут оформляться отдельными защитными мерами.
+ Инструментом для реализации защитной меры следует указать конкретные Межсетевые экраны, если они учитываются в реестре активов - привязать их к карточке в качестве инструментов.

## Связанные угрозы и уязвимости
|Угроза|
|-|
|[Боковое перемещение злоумышленника по локальной сети](/vkr/threats/page1)|

|Уязвимость|
|-|
|[Наличие технических (программных) уязвимостей](/vkr/vulnerabilities/page6)|
