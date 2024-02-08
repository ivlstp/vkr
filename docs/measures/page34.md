# Настройка безопасных заголовков для web сайта

## Описание защитной меры
### Цель: сокращение поверхности для сетевых атак.

Правильная настройка заголовков (headers) веб сервиса полностью или частично защищает его от ряда атак: XSS, CSRF, Clickjacking и иных.
Заголовки могут настраиваться на уровне сайта и/или веб сервера.

Сервис для проверки заголовков: https://securityheaders.com

Перечень заголовков и параметров, которые следует настроить:
- [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options)
- [X-XSS-Protection](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection)
- [Content Security Policy](https://developer.mozilla.org/en-US/docs/Web/HTTP/CSP)
- [Server](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Server) 
- [X-Content-Type-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Content-Type-Options) 
- [X-Download-Options](https://msdn.microsoft.com/en-us/library/jj542450(v=vs.85).aspx)
- [X-Permitted-Cross-Domain-Policies](https://www.adobe.com/devnet/adobe-media-server/articles/cross-domain-xml-for-streaming.html)
- [Referrer-Policy](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Referrer-Policy)
- [Clear-Site-Data](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Clear-Site-Data)
- [HTTP Strict Transport Security](https://developer.mozilla.org/en-US/docs/Web/Security/HTTP_strict_transport_security) 
- [Expect-CT](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Expect-CT)
- [Feature Policy (Permissions-Policy)](https://w3c.github.io/webappsec-feature-policy)
- [Set-Cookie (Secure, HttpOnly)](https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies)
- X-Powered-By

### *Рекомендации к заполнению карточки*:
+ Инструментом для реализации защитной меры следует указать конкретные защищаемые веб-сервисы, если они учитываются в реестре активов - привязать их к карточке в качестве инструментов.
+ В заметке к защитной мере привести инструкции по настройке заголовков используемых в организации веб-сервисов;
+ Создать шаблон регулярной задачи по проверке заголовков у веб-сервисов организации.

## Связанные угрозы и уязвимости
|Угроза|
|-|
|[Заражение вредоносным программным обеспечением](/vkr/threats/page20)|
|[Раскрытие ключей (паролей) доступа](/vkr/threats/page2)|

|Уязвимость|
|-|
|[Возможность проведения межсайтовой подделки запроса CSRF](/vkr/vulnerabilities/page20)|
|[Наличие технических (программных) уязвимостей](/vkr/vulnerabilities/page6)|
