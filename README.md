# Вступление

Этот репозиторий содержит в себе компиляцию вопросов по наступательной безопасности (offensive security). Используя этот материал, можно подготовиться к предстоящему собеседованию или прикинуть какие области знаний Вами не покрыты для самостоятельного обучения. 

Проект является личной инициативой и несет в себе исключительно альтруистические цели. Проект является открытым, каждый желающий может сделать форк или предложить изменения в существующий список вопросов.  Порядок вопросов и их категория носят субъективный характер.  Репозиторий будет наполняться с течением времени, список источников представлен в последнем разделе. Вопросы будут агрегироваться из источников, список источников также будет пополняться. 

# Общие вступительные вопросы

1. Расскажите о себе, о своем опыте, мотивации. В чем выражается интерес к сфере наступательной безопасности?
2. Что вы предпринимаете для личностного и профессионального роста? Как развиваете свои навыки сейчас? Какие ваши источники знаний? 
3. Раскройте понятия "конфиденциальность", "целостность", " доступность " своими словами и приведите примеры.
4. Расскажите о вашей методологии по внутрянке/внешке. Какая последовательность действий у вас выстроилась?
5. Расскройте понятия аутентификации и авторизации. В чем фундаментальные отличия этих понятий? Приведите примеры. Могут ли эти процессы быть независимыми друг от друга? Назовите классификацию факторов аутентификации и назовите примеры.
6. Что такое угроза, уязвимость, эксплойт и меры по устранению?
7. Какую информацию должен включать отчет по тестированию на проникновение?
8. Чем характеризуется атака типа "Отказ в обслуживании". Приведите наглядный пример такой атаки. 
9. Какой тип злоумышленника наиболее опасный: внешний или внутренний?
10. Расскажите о принципе многорубежной защиты (Defense in Depth). В чем его плюсы и минус?  


# Сети

1. Расскажите про модель OSI. Что это такое и для чего нужно?
2. Расскажите про канальный уровень. Чем он характеризуется, какие процессы происходят, какие протоколы здесь присутствуют? Какие атаки возможны?
3. Что такое MAC-адрес? Для чего нужен? Как по MAC-адресу определить вендора? Можно ли менять MAC-адрес и на что это влияет?
4. В чем суть технологии VLAN? Для чего нужно? Какие потенциальные атаки могут совершаться на эту технологию?
5. Расскажите о протоколе ARP? Какие недостатки безопасности есть в этом протоколе? Как работает атака ARP Spoofing?
6. Расскажите о понятии TTL сетевого уровня модели OSI. Для чего этот атрибут нужен? Как по этому параметру может происходить идентификация операционной системы?
7. В чем отличие модели TCP/IP от модели OSI? Какие преимущества и недостатки в каждой из них?
8. Сколько хостов в /27 маске? Как быстро посчитать число устройств для любого префикса?
9. Что такое сетевой порт? Как порт связан с сервисом?
10. Что такое ICMP-flood? На какие параметры атакуемой машины происходит воздействие?
11. Что такое NAT? Какие функции выполняет?
12. Расскажите о протоколе TCP и трехуровневом рукопожатии. Перечислите используемые TCP-флаги в процессе обращения клиента к открытому TCP порту. Что меняется, когда порт становится закрытым?
13. В чем фундаментальные отличия протокола UDP от TCP? Для чего может использоваться UDP?
14. Какую задачу выполняет протокол DNS? Какие типы DNS записей можете перечислить и привести примеры?
15. Что такое передача зоны DNS (DNS Zone Transfer) и как может использоваться злоумышленником?
16. На каком порту работает DNS? Какой/какие протокол/протоколы транспортного уровня используется в DNS? И в каких случаях?
17. Как протокол DNS может использоваться злоумышленниками при DDoS атаках? 
18. Расскажите о стандартах безопасности беспроводных сетей WiFi. От чего зависит выбор стандарта безопасности?
19. Расскажите об известных вам атаках на беспроводные сети WiFi.
20. Расскажите об известных вам атаках на Bluetooth протокол.
21. Расскажите каким образом сетевой сканер nmap определяет открытые порты для TCP и для UDP протоколов. 
22. Расскажите о технике half-handshare (Stealth Scan, -sS в nmap). Почему эта техника является более скрытой нежели обычное TCP-Syn сканиравание?
23. Изменится ли что-то, если запустить nmap с правами суперпользователя (sudo nmap 127.0.0.1)?
24. Расскажите о таких средствах защиты как IDS, IPS. Назовите известные вам решения. Для чего нужны? Какие имеются отличия? Предложите архитектурное решение по внедрению IDS/IPS в корпоративную сеть.
25. Расскройте понятие RADIUS-сервера. Какую задачу решает и как может применяться?



# Операционные системы

## Windows 
1. За что отвечают процессы LSA и LSASS?
2. Что такое база данных SAM? По какому пути лежит и что в ней находится? 
3. Что такое NT-хеш? Как его можно извлечь и что с ним делать? Что такое Pass-The-Hash атака?
4. Что такое NetNTLMv1 / NetNTLMv2 хеши. Чем они отличаются от NT? Как получить NetNTLM хеш и использовать для дальнейшего продвижения?
5. Расскажите про DPAPI ключи. Где они хранятся и для чего используются? Как можно извлечь?
6. Какие топ 5 мер по усилению защиты стандартного Windows-сервера/десктопа?
 
## Linux 
1. Какая информация находится в файле /etc/passwd? Как эта информация может быть использована для повышения привилегий на системе? Что и как влияет на содержимоего этого файла?
2. Что хранится в файле /etc/shadow? Какими привилегиями необходимо обладать для чтения этого файла?
3. Расскажите о переменных окружения. Что это такое и как работает? Дополнительно расскажите о переменной окружения PATH.
4. Что такое SUID-исполняемый файл? Как может использоваться для повышения привилегий в системе?
5. Что такое cron jobs? Как может использоваться для повышения привилегий в системе?
6. О каких уязвимостях ядра Linux вы знаете? Расскажите как они работают
7. Хеши какого типа находятся в файле /etc/shadow? 
8. Какие топ 5 мер по усилению защиты стандартного Linux-сервера/десктопа?


## Контейнеры
1. Что такое контейнер? Есть ли отличия между контейнеризацией и виртуализацией?

# Программирование 
1. Какие функции/методы в языке PHP являются небезопасными и могут привести к выполнению кода?
1. Какие функции/методы в языке Python являются небезопасными и могут привести к выполнению кода?

# Внешка

## Внешние сервисы кроме WEB
1. Расскажите какие сервисы кроме WEB могут быть доступны на внешнем периметре?
2. Расскажите о возможных векторах атак на службу SMTP.

## WEB
1. Расскажите о протоколе HTTP. Клиент-серверная архитектура, методы, заголовки, коды ответов, параметры запросов. 
2. Расскажите какие CMS вам известны? На что направлены векторы атаки в этих CMS?
3. Перечислите какие на ваш взгляд самые важные пункты в OWASP TOP 10 и OWASP TOP 10 API. Приведите примеры. 
4. Отличия тестирования WEB-приложений и API? Какие уязвимости специфичны для подобных приложений?
5. Детально расскажите про несколько типов уязвимостей, например, про XSS (обычные и слепые, хранимые, отраженные и DOM, как обходить фильтрации, какой максимальный импакт возможен), SQL-injections (в том числе second-order, какая более "шумная" - time-based или conditional, и как сделать эксплуатацию менее заметной), CSTI, CSRF.
6. Расскажите про SSRF. Меры защиты и обходы этих мер.
7. Что такое JWT и какие существуют атаки на него?  
8. Расскажите про Insecure Deserialization и последствия. Что такое "magic methods" и "gadget chains". Методы защиты. Есть ли разница в защите клиент-сервер и сервер-сервер.
9. Принцип работы XXE и последствия. Как выполнить XXE OOB и что для этого нужно. Методы защиты. Примеры уязвимых по умолчанию парсеров.
10. Расскажите о возможных уязвимостях в функционале загрузке файлов. Возможные варианты защиты и обхода защиты.
11. Расскажите о возможных атаках на стандарт OAuth2.
12. CORS, SOP, CSP, Security Headers. Для чего они нужны и как корректно должны быть настроены? Отличия SameSite от SameOrigin. 
13. Небезопасная десериализация в различных языках программирования. Какие библиотеки и в каких языках программирования подвержены ей? В каких случаях и какого импакта возможно добиться?
14. Расскажите о более специфичные уязвимости - CSS-инъекция, XSSI, XSLT, Prototype Pollution.
15. Что такое WAF? Как работает и какие распространенные методы обхода существуют?


# Внутрянка

## Active Directory
1. Расскажите о протоколе LDAP. Для чего и как используется?
2. Расскажите о службе ADCS. Для чего и как используется? Каким атакам может быть подвержен?
3. Расскажите о службе Kerberos. Для чего и как используется? Назовите этапы протокола Kerberos для прохождения аутентификации на сервере приложений. Каким атакам может быть подвержен протокол?
4. Расскажите о сетевой папке SYSVOL. Где она находится в домене ActiveDirectory, для чего предназначена, какие мисконфиги могут быть тут найдены?
4. Каким bloodhound-сбощиком пользуетесь? Назовите известные вам рёбра (edges) в bloodhound и как их эксплуатировать?
5. Расскажите концептуально про Relay-атаки. В каких случаях и с какими протоколами это возможно? Какие есть ограничения и меры защиты от такой атаки?
6. Расскажите об известных вам механизмах закрепления в Active Directory?
7. Расскажите про атаку LDAP-PassBack. В каких случаях это возможно?
8. Какие методы аутентификации в Active Directory помимо пароля вы знаете?

# Облака

1. Расскройте понятия IaaS, PaaS, SaaS. 
2. Назовите известных вам облачных провайдеров.
3. Какие риски накладываются на потребителя услуг при использовании облачной инфраструктуры?

# Криптография
1. Расскажите как работает ассиметричная и симметричная криптография на базовом уровне. Назовите примеры симметричного и ассиметричного криптографического алгоритма. 
2. Расскажите о роли цепи Фейстеля в симметричной криптографии. 
2. Приведите примеры криптографических и некриптографических хеш-функций. Какие могут быть области применения у первых и вторых?
3. Приведите примеры небезопасных хеш-функций для задач защиты пароля в базе данных
4. Назовите основные свойства криптографической хеш-функций. 
5. Расскажите о протоколе TLS применительно к HTTP.
6. Почему протоколы SSL 1.0, SSL 2.0, SSL 3.0 являются небезопасными?
7. Расскажите о протоколе обмена ключами Диффи-Хеллмана. Как работает и каким атакам подвержена базовая реализация?
7. Расскажите о сути атаки Padding Oracle.
8. Какие атаки на RSA вам известны? 
9. Расскажите об отличаях потокового и блочного шифра в симметричной криптографии. 
10. Расскажите об алгоритме BPKDF. Для чего используется и какую отличительную особенность имеет?
11. Расскажите о примитивах MAC/HMAC в терминах криптографии. Для чего нужны и какие свойства присутствуют.
12. Что такое криптографическая соль и криптографический перец? В чем отличие и какие задачи решают?

# OSINT

1. Назовите используемые вами инструменты технической пассивной разведки.
2. Что такое HumINT, какие средства могут использоваться для такого вида разведки?
3. Какую информацию можно получить из TLS сертификата?
4. Какую информацию можно получить из DNS записей исследуемого домена?
5. Что такое Certificate Transparency в TLS сертификатах и как это свойство может использоваться для задач OSINT?
6. Какая информация может быть получена о юридическом лице и какими источниками вы бы воспользовались?

# Социальная инженерия

1. Расскажите и привидите примеры социальных атак по классификации канала доставки (почта, телефон, мессенджер и т.д.)?
2. Расскажите какие типы полезных нагрузок могут быть использованы в ходе атак методами социальной инженерии?
3. Какими инструментами пользуетесь для реализации атаки методом социальной инженерии?

# Мобилки

Эта секция вопросов посвящена безопасности мобильных приложений. Затрагиваются вопросы динамического и статического тестирования.

1. Какие вы знаете подходы к хранению данных приложения, как наиболее безопасно хранить данные и как атаковать небезопасное хранение в различных конфигурациях

## Android

1. Дано название мобильного приложения. Какие способы получения APK файла вы знаете? 
2. Что такое AndroidManifest файл? Что в нем находится и как может быть полезно при исследовании безопасности мобильного приложения?
3. Назовите основные компоненты android приложения.
4. В чем опасность экспортируемых компонентов?
5. Назовите несколько способов вызова экспортируемых компонентов.
6. Какими способами можно обойти проверку наличия root-прав в приложении?
7. Что такое SSL-Pinning? От чего защищает? Какими способами может быть реализован?
8. 

## iOS


# Источники
| Номер | URL                                                              |
| ----- | ---------------------------------------------------------------- |
| 1 [x]     | https://itanddigital.ru/interviewsecurity                        |
| 2 [x]    | https://github.com/redteamcaptain/Pentesting-Interview-Questions |
| 4 [x]    | https://t.me/pain_test/64                                        |
| N     | https://t.me/pathsecure_chat                                     |

# Контрибьюторы списком
- https://t.me/cherepawwka
- https://t.me/Haones
- https://t.me/FuckingMoneyToiletPaper
- https://t.me/zhatez
- https://t.me/curiv
- https://t.me/W0lFreaK
