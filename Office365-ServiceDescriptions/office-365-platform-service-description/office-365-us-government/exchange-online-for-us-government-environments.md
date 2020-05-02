---
title: Exchange Online для сред США для государственных организаций
ms.author: sharik
author: skjerland
manager: mnirkhe
audience: ITPro
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ms.custom: Adm_ServiceDesc
description: В этой статье представлены общие сведения о различиях между функциями Cloud правительства США и коммерческой облаком, указанным в описании службы Exchange Online.
ms.openlocfilehash: f104f072a74707f46528d9b111d8af46103a919e
ms.sourcegitcommit: 87c1b1cc9c02e5f446e382f1174cbbccad20196d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/25/2020
ms.locfileid: "43813409"
---
# <a name="exchange-online-for-us-government-environments"></a>Exchange Online для сред США для государственных организаций

В этой статье представлены общие сведения о различиях между функциями Cloud правительства США и коммерческой облаком, указанным в [описании службы Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-service-description). Exchange Online доступен для сред, в которых используется облако сообщества для государственных организаций (GCC), GCC High и Department of обороны (DoD).

Дополнительные сведения о правительственном облаке, включая сведения о приемлемости и приобретении, можно найти [в статье Microsoft 365 государственных учреждений — как приобрести](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/microsoft-365-government-how-to-buy). Чтобы сравнить планы Office 365 для государственных учреждений, ознакомьтесь с [планами office 365 для государственных организаций](https://www.microsoft.com/microsoft-365/government/compare-office-365-government-plans?rtc=1#EligibilityRequirements).

Чтобы узнать о необходимых конечных точках при управлении подключением к сети, ознакомьтесь со статьями [Office 365 для государственных учреждений GCC gcc High](https://docs.microsoft.com/office365/enterprise/office-365-u-s-government-gcc-high-endpoints#sharepoint-online-and-onedrive-for-business) , а также [конечных точек DOD Office 365 для правительства США](https://docs.microsoft.com/office365/enterprise/office-365-u-s-government-dod-endpoints#sharepoint-online-and-onedrive-for-business).

В дополнение к преимуществам функций и возможностей Office 365 организации могут использовать следующие функции, уникальные для облачных сред США:

- Контент клиента вашей организации логически отделяется от контента клиентов в коммерческих службах Office 365.

- Контент клиентов вашей организации хранится в оставшейся части США.

- Доступ к контенту клиентов вашей организации ограничен защищенным персоналом корпорации Майкрософт.

- Облачные среды для государственных организаций соответствуют сертификациям и аттестационных программ, необходимым для пользователей с общественным сектором США.

В облачной среде для государственных организаций все функции и функции Exchange предоставляются по общему преднамеренному преднамерению. С другой стороны, некоторые функции недоступны в связи с требованиями клиентов государственных организаций. Другие функции поступают в государственные среды, но еще не доступны. Ознакомьтесь со следующими разделами, чтобы узнать о доступности функций в облачных средах государственных организаций.

## <a name="exchange-online-features"></a>Функции Exchange Online 

В приведенной ниже таблице указано, доступны ли указанные функции Exchange Online в средах GCC, GCC High и DoD. При наличии нюансов, касающихся оператора поддержки (или его недостает), предоставляется дополнительный контекст.

|**Область функций**|**GCC**|**GCC High**|**Вызов**|**Ключевые моменты**|
|:-----|:-----|:-----|:-----|:-----|
|**[Планирование и развертывание](../../exchange-online-service-description/planning-and-deployment.md)**|||||
|Поддерживается гибридное развертывание|Да|Да|Да|Для совместного использования с локальным сервером Exchange Server корпорации Майкрософт требуется установить по крайней мере один сервер клиентского доступа Exchange Server 2013 (или Exchange Server 2016.). Exchange Server 2010 и более ранние версии не поддерживаются.|
|Поддерживается миграция IMAP|Да|Да|Да||
|Поддержка прямой миграции|Да|Да|Да||
|Поддерживается поэтапная миграция|Да|Да|Да|Гсуите миграция не поддерживается для GCC High и DoD. Дополнительные сведения см. <a href="https://docs.microsoft.com/exchange/mailbox-migration/perform-g-suite-migration">в статье выполнение гсуите миграции</a>.|
|**[Разрешения](../../exchange-online-service-description/permissions.md)**|**GCC**|**GCC High**|**Вызов**|**Ключевые моменты**|
|Разрешения на основе ролей|Да|Да|Да||
|Группы ролей|Да|Да|Да||
|Политики назначения ролей|Да|Да|Да||
|**[Политика обработки сообщений и соответствие требованиям](../../exchange-online-service-description/message-policy-and-compliance.md)**|**GCC**|**GCC High**|**Вызов**|**Ключевые моменты**|
|Архивация почтовых ящиков на основе Exchange Online|Да|Да|Да||
|Архивация сообщений в облаке для локальных почтовых ящиков|Да|Да|Да||
|Messaging Records Management (MRM) |Да|Да|Да||
|Ручные политики хранения, метки и Теги |Да|Да|Да||
|Шифрование статических данных (BitLocker)|Да|Да|Да||
|IRM на базе Azure Information Protection|Да|Да|Да|Для получения дополнительных сведений об ограничениях АДМИНИСТРАТИВной установки в GCC High и DoD обратитесь к статье <a href="https://docs.microsoft.com/enterprise-mobility-security/solutions/ems-aip-premium-govt-service-description">Описание службы Azure Information Protection Premium</a>.<br><br>Azure Information Protection не входит в G1/F3, но ее можно приобрести как отдельную надстройку и включить поддерживаемые функции управления правами на доступ к данным (IRM). Некоторые функции Azure Information Protection требуют подписки на Office 365 профессиональный плюс, которые не входят в состав Office 365 для государственных учреждений G1 или Office 365 для государственных учреждений 3.|
|Управление правами на доступ к данным с помощью AD RMS для Windows Server|Да|Да|Да|Windows Server AD RMS — это локальный сервер, который необходимо приобрести отдельно, чтобы включить поддерживаемые функции IRM.|
|Шифрование сообщений Office 365|Да|Да|Да|В этой статье описывается [поведение шифрования сообщений в office 365](#office-365-message-encryptionbehavior-across-gcc-highdod-boundary) , а также <a href="https://docs.microsoft.com/microsoft-365/compliance/ome-version-comparison?view=o365-worldwide#unique-characteristics-of-office-365-message-encryption-in-a-gcc-high-deployment">уникальные характеристики шифрования сообщений Office 365 при высоком развертывании GCC</a>, которые задокументированы особенности использования шифрования сообщений Office 365 при отправке сообщений между пользователями GCC High/DOD и не GCC High/DOD.|
|Ключ клиента|Да|Да|Да|Требуется план обслуживания G5.|
|S/MIME|Да|Да|Да||
|Хранение на месте и хранение для судебного разбирательства|Да|Да|Да|Требуется план обслуживания G3 или G5.|
|Обнаружение электронных данных на месте|Да|Да|Да||
|Правила потока обработки почты|Да|Да|Да||
|Защита от потери данных|Нет|Да|Да|Требуется план обслуживания G3 или G5.|
|Ведение журнала|Да|Да|Да||
|**[Защита от нежелательной почты и вредоносных программ](../../exchange-online-service-description/anti-spam-and-anti-malware-protection.md)**|**GCC**|**GCC High**|**Вызов**|**Ключевые моменты**|
|Встроенная защита от нежелательной почты|Да|Да|Да||
|Customize anti-spam policies|Да|Да|Да||
|Встроенная защита от вредоносных программ|Да|Да|Да||
|Customize anti-malware policies|Да|Да|Да||
|Карантин  управление администраторами|Да|Да|Да||
|Карантин  самостоятельное управление пользователями|Да|Да|Да||
|Расширенная защита от угроз|Да|Да|Да|Требуется план обслуживания G5 (или приобрести надстройку).<br><br>Защита от фишинга для олицетворения пользователя и домена и логики подмены пока недоступна в GCC High и DoD.|
|**[Поток обработки почты](../../exchange-online-service-description/mail-flow.md)**|**GCC**|**GCC High**|**Вызов**|**Ключевые моменты**|
|Настраиваемая маршрутизация исходящей почты|Да|Да|Да||
|Secure messaging with a trusted partner|Да|Да|Да||
|Conditional mail routing|Да|Да|Да||
|Добавление партнера в список входящих безопасных надежных отправителей|Да|Да|Да||
|Маршрутизация почты в гибридной конфигурации|Да|Да|Да||
|**[Получатели](../../exchange-online-service-description/recipients.md)**|**GCC**|**GCC High**|**Вызов**|**Ключевые моменты**|
|Оповещения о доступном объеме|Да|Да|Да||
|Папка "Несрочные"|Да|Да|Да||
|Подсказки|Да|Да|Да||
|Делегированный доступ|Да|Да|Да||
|Правила для папки "Входящие"|Да|Да|Да||
|Подключенные учетные записи|Да|Нет|Нет|Эта функция не поддерживается в GCC High или DoD из-за ограничений для исходящих подключений к сторонним службам. Более подробную информацию о возможностях можно узнать в статье [Подключение к сторонним службам](#connectivity-with-third-party-services) в этой статье.|
|Неактивные почтовые ящики|Да|Да|Да|Требуется план обслуживания G3 или G5.|
|Автономная адресная книга|Да|Да|Да||
|Политики адресных книг|Да|Да|Да||
|Иерархическая адресная книга|Да|Да|Да||
|Списки адресов и глобальный список адресов|Да|Да|Да||
|Группы Office 365|Да|Да|Да|Гостевой доступ к группам Office 365 не поддерживается в средах GCC High и DoD. Дополнительные сведения см. в статье <a href="https://docs.microsoft.com/azure/azure-government/documentation-government-services-securityandidentity">безопасность и удостоверение в Azure</a>.|
|Группы рассылки|Да|Да|Да||
|Внешние контакты (глобальный список)|Да|Да|Да|Подчиняются ограничениям для совместной работы с организационными отношениями в средах GCC High и DoD. |
|Связывание контактов с социальными сетями|Да|Нет|Нет|Эта функция не поддерживается в GCC High или DoD.|
|Почтовые ящики ресурса|Да|Да|Да||
|Управление конференц-залами|Да|Да|Да||
|Ответы об отсутствии на работе|Да|Да|Да||
|Общий доступ к календарю в Интернете|Да|Нет|Нет|В GCC High публикация и общий доступ к календарю в Интернете работают для входящих подключений к календарям, которые доступны пользователям GCC High, но не для большинства пользователей GCC, подключающихся к общему календарю за предельное значение GCC High.<br><br>В целях DoD — общий доступ к Интернет-календарю не поддерживается из-за того, что требование для входящего и исходящего подключения разрешено для списка в этой среде.|
|**[Функции создания отчетов и средства устранения неполадок](../../exchange-online-service-description/reporting-features-and-troubleshooting-tools.md)**|**GCC**|**GCC High**|**Вызов**|**Ключевые моменты**|
|Отчеты центра администрирования Microsoft 365|Да|Да|Нет|Отчеты, недоступные для вызова по требованию. Для получения обновлений и текущей доступности обратитесь к разделу <a href="https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government#platform-features">функции платформы</a> в описании службы Office 365 США для государственных организаций.|
|Отчеты веб-служб|Да|Да|Нет|Отчеты, недоступные для вызова по требованию. Для получения обновлений и текущей доступности обратитесь к разделу <a href="https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government#platform-features">функции платформы</a> в описании службы Office 365 США для государственных организаций.|
|Message trace|Да|Да|Да||
|Отчеты аудита|Да|Да|Нет|Отчеты, недоступные для вызова по требованию. Для получения обновлений и текущей доступности обратитесь к разделу <a href="https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government#platform-features">функции платформы</a> в описании службы Office 365 США для государственных организаций.|
|Отчеты единой системы обмена сообщениями|Да|Нет|Нет||
|**[Общий доступ и совместная работа](../../exchange-online-service-description/sharing-and-collaboration.md)**|**GCC**|**GCC High**|**Вызов**|**Ключевые моменты**|
|Федеративный общий доступ (включая публикацию календаря)|Да|Да|Да|Существуют ограничения как для GCC High, так и для DoD. В этой статье вы найдете сведения об [Федерации сведений о доступности](#freebusy-federation) .|
|Почтовые ящики сайта|Да|Да|Да||
|Общедоступные папки|Да|Да|Да||
|**[Клиенты и мобильные устройства](../../exchange-online-service-description/clients-and-mobile-devices.md)**|**GCC**|**GCC High**|**Вызов**|**Ключевые моменты**|
|Outlook для Windows|Да|Да|Да|Чтобы удовлетворить требования к высокой и несоответствию требованиям GCC, необходимо использовать по крайней мере 1803 Office 365 профессиональный плюс. Office 365 профессиональный плюс не входит в состав G1 или F3.|
|Outlook в Интернете|Да|Да|Да||
|Outlook для Mac|Да|Да|Да|Чтобы удовлетворить требования к высокой и несоответствию требованиям GCC, необходимо использовать по крайней мере 1803 Office 365 профессиональный плюс. Office 365 профессиональный плюс не входит в состав G1 или F3.|
|Outlook для iOS и Android|Да|Да|Да||
|Exchange ActiveSync|Да|Да|Да||
|Управление мобильными устройствами для Office 365|Да|Да|Да||
|POP и IMAP|Да|Да|Да||
|SMTP|Да|Да|Да||
|Поддержка приложений EWS|Да|Да|Да||
|**[Службы голосовых сообщений](../../exchange-online-service-description/voice-message-services.md)**|**GCC**|**GCC High**|**Вызов**|**Ключевые моменты**|
|Голосовая почта|Нет|Нет|Нет|Интеграция локальных систем IP-УАТС с единой системой обмена сообщениями Exchange Online не поддерживается.|
|Интеграция голосовой почты и стороннего ФАКСа|Нет|Нет|Нет|Интеграция локальных систем IP-УАТС с единой системой обмена сообщениями Exchange Online не поддерживается.|
|Взаимодействие со сторонней голосовой почтой|Нет|Нет|Нет|Интеграция локальных систем IP-УАТС с единой системой обмена сообщениями Exchange Online не поддерживается.|
|Интеграция со Skype для бизнеса|Да|Да|Да||
|**[Высокая доступность и непрерывность бизнес-процессов](../../exchange-online-service-description/high-availability-and-business-continuity.md)**|**GCC**|**GCC High**|**Вызов**|**Ключевые моменты**|
|Репликация почтовых ящиков в центрах обработки данных|Да|Да|Да||
|Восстановление удаленного почтового ящика|Да|Да|Да||
|Восстановление удаленных элементов|Да|Да|Да||
|Восстановление отдельных элементов|Да|Да|Да||
|**[Взаимодействие, связь и совместимость](../../exchange-online-service-description/interoperability-connectivity-and-compatibility.md)**|**GCC**|**GCC High**|**Вызов**|**Ключевые моменты**|
|Присутствие в OWA и Outlook|Да|Да|Да||
|Взаимодействие с SharePoint|Да|Да|Да||
|Поддержка подключения EWS|Да|Да|Да||
|Поддержка ретрансляции SMTP|Да|Да|Да||
|**[Установка и администрирование Exchange Online](../../exchange-online-service-description/exchange-online-setup-and-administration.md)**|**GCC**|**GCC High**|**Вызов**|**Ключевые моменты**|
|Доступ к порталу Microsoft Office 365|Да|Да|Нет|Отчеты, недоступные для вызова по требованию. Для получения обновлений и текущей доступности обратитесь к разделу <a href="https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government#platform-features">функции платформы</a> в описании службы Office 365 США для государственных организаций.|
|Доступ к центру администрирования Microsoft 365|Да|Да|Нет|Отчеты, недоступные для вызова по требованию. Для получения обновлений и текущей доступности обратитесь к разделу <a href="https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government#platform-features">функции платформы</a> в описании службы Office 365 США для государственных организаций.|
|Доступ к Центру администрирования Exchange|Да|Да|Да||
|Удаленный доступ к Windows PowerShell|Да|Да|Да||
|Политики ActiveSync для мобильных устройств|Да|Да|Да||
|Отчеты об использовании|Да|Да|Нет|Отчеты, недоступные для вызова по требованию. Для получения обновлений и текущей доступности обратитесь к разделу <a href="https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government#platform-features">функции платформы</a> в описании службы Office 365 США для государственных организаций.|
|**[Расширение настройки службы, надстроек и ресурсов](../../exchange-online-service-description/exchange-online-service-description.md)**|**GCC**|**GCC High**|**Вызов**|**Ключевые моменты**|
|Надстройки Outlook и Outlook MAPI|Да|Да|Да|Только некоторые надстройки OWA и Outlook доступны в GCC High и DoD. В этой статье представлены надстройки [в Outlook и Outlook Web App](#add-insin-outlook-and-outlook-web-app) .|

## <a name="feature-nuances-within-gcc-high-and-dod-environment"></a>Особенности функций в среде High and DoD

### <a name="connectivity-with-third-party-services"></a>Связь со сторонними службами  

Как самые высокие, так и DoD среды используют ограниченные среды, требующие явного утверждения и настройки исходящих подключений. Кроме того, корпорация Майкрософт не может разместить запросы на разрешение исходящего доступа из этих сред в коммерческие облачные службы (коммерческая версия Office 365, Google Гсуите, веб-службы Amazon и т. д.).     

В связи с этими ограничениями функции, зависящие от этого исходящего подключения из сред с поддержкой GCC High и DoD, обычно не поддерживаются, в том числе: 

- Подключенные&mdash;учетные записи пользователи не могут добавлять или синхронизировать учетные записи (Google, POP/IMAP и т. д.). 

- Поддержка сторонних поставщиков&mdash;хранилища файлов для учетной записи пользователя в OneDrive для бизнеса с помощью *GCC High/DOD* можно получить доступ из различных клиентов Outlook в целях присоединения и предоставления общего доступа к файлам. Нельзя добавить сторонние учетные записи хранения (Dropbox, Box, Google Drive). 

- Связь с социальными сетями, такими как Facebook и LinkedIn. 

### <a name="azure-active-directoryb2b-collaboration"></a>Совместная работа Azure Active Directory B2B 

В настоящее время совместная работа Azure Active Directory B2B поддерживается только между организациями, которые находятся в облаке Azure США и поддерживают совместную работу по B2B.

Кроме того, пользователи B2B, являющиеся гостями в группах Office 365, не поддерживаются в средах GCC High и DoD. 

Дополнительные сведения и последние обновления можно найти в статье [безопасность и удостоверение в Azure для государственных учреждений](https://docs.microsoft.com/azure/azure-government/documentation-government-services-securityandidentity). 

### <a name="office-365-message-encryptionbehavior-across-gcc-highdod-boundary"></a>Поведение шифрования сообщений в Office 365 для границ GCC High/DoD 

Если вы хотите использовать шифрование сообщений Office 365 в среде с большим числом GCC, учитывайте следующие уникальные характеристики взаимодействия с получателем:  

- При отправке зашифрованных сообщений электронной почты из GCC High или DoD для получателей в одной и той же среде:
    
    - Отправители могут вручную зашифровывать сообщения в Outlook для ПК и Mac, а также Outlook в Интернете, а организации могут настраивать политику для шифрования электронных сообщений с помощью правил для почтовых ящиков Exchange. 
    
    - Получатели в пределах GCC High/DoD получают одинаковый режим чтения в Outlook для компьютеров с Windows и Mac и Outlook в Интернете, как и все остальные пользователи Office 365. 

<!-- end list -->

- При отправке зашифрованных сообщений электронной почты из GCC High или DoD для получателей, не входящих в эту среду (включая GCC и коммерческая версия):
    
    - Отправители внутри GCC High/DoD могут отправлять зашифрованную электронную почту за пределами границы GCC High/DoD. 
    
    - Все получатели, не относящиеся к Microsoft GCC High/DoD, в том числе коммерческие пользователи Office 365, пользователи Outlook.com и другие пользователи других поставщиков электронной почты, получают сообщения программы-оболочки. Эта почтовая оболочка перенаправляет получателя на портал OME, где получатель может прочитать сообщение и ответить на него. 

Дополнительные сведения и последние обновления приведены в статье [Сравнение версий OME](https://docs.microsoft.com/microsoft-365/compliance/ome-version-comparison?view=o365-worldwide).

### <a name="freebusy-federation"></a>Федерация сведений о доступности

Для федеративного общего доступа, в том числе сведений о доступности, в настоящее время действуют некоторые важные ограничения в средах GCC High и DoD.

В высокой среде GCC:

- Доверие федерации (включая двунаправленный обмен сведениями о доступности) поддерживается между клиентами в GCC High и с помощью гибридной сосуществования (Exchange 2013 или более поздней версии).

- Федеративный общий доступ не поддерживается между клиентами в GCC High и GCC или Office 365 для коммерческих организаций. Исходящие подключения от высокой среды GCC к коммерческим облакам (включая GCC и Office 365 Профессиональная) в настоящее время не разрешены. В результате пользователи GCC High не смогут отправить сведения о доступе к общему календарю.

В среде DoD:

  - Доверие федерации (включая общий доступ к сведениям о доступности) в настоящее время поддерживается только между клиентами в среде DoD. Он не поддерживается между клиентами DoD и коммерческими клиентами GCC или коммерческими клиентами.

### <a name="client-configuration"></a>Настройка клиента 

Дополнительные действия участвуют в развертывании и настройке Office профессиональный плюс (включая Outlook). Подробное описание этих действий приведено [в статье рекомендации по развертыванию приложений Microsoft 365 для предприятий в среде с контрастной или с Microsoft GCC High или DOD ](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-gcc-high-dod).

Outlook для iOS и Android также доступны в средах GCC High и DoD. Дополнительные сведения об ограничениях функций и управлении в этих средах приведены [в статье Использование Outlook для iOS и Android в облаке сообщества государственных организаций](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/outlook-for-ios-and-android/outlook-for-ios-and-android-in-the-government-cloud).

### <a name="add-insin-outlook-and-outlook-web-app"></a>Надстройки в Outlook и Outlook Web App  

Только некоторые надстройки OWA и Outlook доступны в GCC High и DoD. Мои шаблоны и предлагаемые собрания доступны и должны работать. Поддерживаются только пять надстроек OWA по умолчанию. Однако интеграция с приложениями сторонних производителей возможна, однако эти интеграции не охватываются корпорацией Майкрософт, обещанными корпорацией Майкрософт для GCC High или DoD. Пользователи должны ознакомиться с практическими рекомендациями по управлению данными и соответствием требованиям, прежде чем настраивать надстройку для своей организации.