# Возможность атаки Man in the Browser

## Описание уязвимости
Атака Man in the Browser - это когда злоумышленник внедряет в браузер программное обеспечение, которое позволяет ему получать файлы cookie, сеансы HTTP и сертификаты SSL пользователя, использовать браузер в качестве способа перехода во внутреннюю сеть.
Трафик перенаправляется из браузера злоумышленника через браузер пользователя путем настройки HTTP-прокси, который перенаправляет любой HTTP-и HTTPS-трафик. Браузеры обычно создают новый процесс для каждой открываемой вкладки, и разрешения и сертификаты разделяются соответствующим образом. С этими разрешениями злоумышленник может перейти к любому ресурсу в интрасети, доступному через браузер и имеющему достаточные разрешения, например Sharepoint или веб-почту. Перенаправление трафика через браузер может обходить двух-факторную аутентификацию.

## Вхождение в базы ФСТЭК, MITRE ATT&CK
### Техники MITRE ATT&CK:
+ T1185 Browser Session Hijacking

## Связанные угрозы
|Угроза|
|-|
|[Утечка информации](/vkr/threats/page11)|