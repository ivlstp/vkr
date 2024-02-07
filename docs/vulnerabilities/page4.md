# Публикация информации в открытых источниках

В Интернете множество свободно доступных технических баз данных аккумулирующих информацию о компаниях: регистраторы доменов, цифровые сертификаты, публичные сканеры (например shodan.io), сайты и социальные сети компании.
В большинстве случаев представленная там информация должна быть публично доступна для исправного функционирования активов компании.
Часть информации может быть использована злоумышленниками для развития атаки на компанию: адреса электронной почты, IP адреса, домены, информация о технической реализации публичных сервисов, учетные записи пользователей, имена и должности сотрудников.

### Техники MITRE ATT&CK:
+ T1589 Gather Victim Identity Information
+ T1589.002 Gather Victim Identity Information: Email Addresses
+ T1589.003 Gather Victim Identity Information: Employee Names
+ T1596 Search Open Technical Databases
+ T1596.001 Search Open Technical Databases: DNS/Passive DNS
+ T1596.002 Search Open Technical Databases: WHOIS
+ T1596.003 Search Open Technical Databases: Digital Certificates
+ T1596.004 Search Open Technical Databases: CDNs
+ T1596.005 Search Open Technical Databases: Scan Databases