---
title: Получатели
ms.author: office365servicedesc
author: pamelaar
audience: ITPro
ms.topic: reference
f1_keywords:
- exchange-online-recipients
ms.service: o365-administration
localization_priority: Normal
ms.custom: Adm_ServiceDesc
ms.assetid: da22b03a-c981-49c6-9928-4312c2c5e2ee
description: В этой статье описаны компоненты Microsoft Exchange Online, связанные с получателями. Сюда относятся электронная почта, контакты, группы рассылки, а также календарь и возможности планирования.
ms.openlocfilehash: 5156272ea444414b8da650cf294f99bdfb8b4081
ms.sourcegitcommit: e342174df76128430dfc8c971716da5c4b2942ac
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2020
ms.locfileid: "48293865"
---
# <a name="recipients"></a>Получатели

В этой статье описаны компоненты Microsoft Exchange Online, связанные с получателями. Сюда относятся электронная почта, контакты, группы рассылки, а также календарь и возможности планирования.
  
## <a name="email"></a>Электронная почта

Каждый подписчик Microsoft Exchange Online получает каждый почтовый ящик; кроме того, доступны особые почтовые ящики для планирования использования ресурсов (например, конференц-залов) и многопользовательского доступа к общим почтовых адресам. Ограничения на максимальную емкость подсистемы хранения распространяются на большинство почтовых ящиков, и администраторы могут контролировать допустимый размер почтовых ящиков. Автоматизированные уведомления и ограничения могут оповещать пользователей, если размер их почтовых ящиков приближается к пределу. Служба Exchange Online также содержит несколько типов ограничений — размер сообщений, скорость обмена сообщениями и списки получателей. Ниже приводится подробная информация обо всех этих функциях и ограничениях.
  
> [!NOTE]
> Адреса регистрации всех сообщений больше не поддерживаются в Exchange Online. Из-за фильтрации получателей для защиты от возможных нежелательных сообщений адреса электронной почты, которые не существуют в вашей организации, будут отклонены. 
  
### <a name="mailbox-types-storage-limits-and-capacity-alerts"></a>Типы почтовых ящиков, пределы хранения и оповещения о доступном объеме

Объем хранилища почтовых ящиков, доступный пользователю, а также размер почтового ящика по умолчанию определяются типом почтового ящика и лицензией подписки пользователя. Администраторы могут уменьшить максимальный размер почтовых ящиков отдельного пользователя или глобально. Exchange Online отображает оповещения, когда в почтовом ящике пользователя мало места или он заполнен.
  
Для получения дополнительных сведений см раздел "пределы хранилища почтовых ящиков" и "оповещения о емкости" в разделе " [Exchange Online Limits](exchange-online-limits.md)".
  
### <a name="mailtips"></a>Подсказки

Подсказки  это автоматические информационные сообщения, которые появляются над полем "Кому", когда пользователи создают сообщения. Они помогают предотвратить случайную доставку, нарушение политик и отчеты о недоставке (NDR). Например, они появляются, когда пользователи отправляют сообщения в чрезмерно большие группы, группы, содержащие внешних получателей, или группу рассылки с модерацией или ограничениями. Дополнительные сведения см. в статье [Подсказки](https://go.microsoft.com/fwlink/p/?LinkId=401472).
  
### <a name="delegate-access"></a>Делегированный доступ

Exchange Online поддерживает делегирование доступа  возможность пользователей разрешить другим пользователям управлять своей электронной почтой и календарями. Передача прав доступа обычно используется между руководителем и помощником, где помощник обрабатывает входящие сообщения электронной почты и координирует расписание руководителя. Делегированный доступ может быть включен пользователями Exchange Online в Outlook или Outlook в Интернете или администраторами в центре администрирования Exchange. 
  
Делегаты могут иметь два вида доступа:
  
- **Разрешения на отправку от имени другого лица** Делегат может составить сообщение электронной почты и ввести имя другого пользователя в поле "От", где он будет отображаться в виде "[имя делегата] от имени [имя пользователя]". 
    
- **Разрешения "Отправить как"** Делегат может отправлять сообщения от имени другого пользователя, как если бы делегат почтового ящика был владельцем почтового ящика. Этот сценарий распространен там, где есть общий почтовый ящик и несколько сотрудников отправляют сообщения электронной почты из почтового ящика, а не из своих учетных записей Exchange Online. 
    
Подробную информацию о делегировании прав доступа см. в статье [Управление разрешениями для получателей](https://technet.microsoft.com/library/jj919240%28v=exchg.160%29.aspx).
  
### <a name="inbox-rules"></a>Правила для папки "Входящие"

Служба Exchange Online позволяет создавать правила для папки входящих сообщений для автоматического выполнения определенных действий над сообщениями на основе критериев в момент их поступления. Например, пользователи могут создать правило для автоматического перемещения всей почты в определенную папку, если почта было отправлена в определенную группу рассылки. Пользователи управляют правилами папки "Входящие" из Outlook или Outlook в Интернете. Администраторы могут блокировать определенные типы правил для папки входящих сообщений на сервере, отключив переадресацию или серверные автоматические ответы. Например, отключение переадресации почты со стороны сервера позволяет предотвратить автоматическую пересылку электронной почты на личные учетные записи. Аналогично, отключение автоматических ответов со стороны сервера позволяет предотвратить автоматические ответы внешним сторонам и возможность идентификации допустимых адресов электронной почты. Эти изменения вносятся через удаленную консоль Windows PowerShell.
  
### <a name="clutter"></a>Папка "Несрочные"

Функция "Несрочные" помогает сосредоточиться на важных сообщениях. С помощью технологии машинного обучения она перемещает сообщения с низким приоритетом из папки "Входящие" в новую папку "Несрочные". Эта функция учитывает существующие правила электронной почты. Если вы создавали их для упорядочивания почты, они продолжат действовать. По умолчанию функция "Несрочные" в папке "Входящие" отключена. Дополнительную сведения см. в статье [Как упорядочить сообщения в папке "Входящие" в Office 365](https://go.microsoft.com/fwlink/?linkid=2144145).
  
### <a name="connected-accounts"></a>Подключенные учетные записи

Функция подключенных учетных записей позволяет пользователям Exchange Online связывать внешние учетные записи электронной почты (например, личные учетные записи) с их внутренними учетными записями электронной почты в Exchange Online, а затем использовать Outlook в Интернете для взаимодействия со всеми сообщениями в одном месте. Подключенные учетные записи автоматически синхронизируются при входе в Outlook в Интернете; Кроме того, пользователи могут вручную синхронизировать учетные записи из Outlook в Интернете. Администраторы могут включать и отключать эту функцию для определенных пользователей или всех пользователей с помощью [центра администрирования Exchange](https://go.microsoft.com/fwlink/?LinkID=785297&amp;clcid=0x409).
  
### <a name="inactive-mailboxes"></a>Неактивные почтовые ящики

Exchange Online позволяет сохранять содержимое удаленных почтовых ящиков в течение неопределенного времени. Эта функция называется Неактивные почтовые ящики. Почтовый ящик становится неактивным, когда к нему применяется хранение на месте или хранение для судебного разбирательства перед удалением. В результате этого действия содержимое данного почтового ящика хранится в течение неограниченного времени. Администраторы, сотрудники, ответственные за обеспечение соответствия требованиям, или управляющие записями могут получать доступ к содержимому неактивных почтовых ящиков с помощью функции обнаружения электронных данных в Exchange Online.
  
Для включения функции неактивного почтового ящика требуется, чтобы ящик имел активную лицензию Exchange Online (план 2) или подписку на архивацию на базе Exchange Online,  только в этом случае возможно применение функции хранения на месте или хранения для судебного разбирательства к почтовому ящику перед его удалением.
  
> [!IMPORTANT]
> Если функция хранения не применена к почтовому ящику до его удаления, содержимое этого почтового ящика не сохраняется и не сможет быть обнаружено. Почтовый ящик можно восстановить в течение 30 дней с момента удаления, при этом если в данный промежуток времени восстановление не будет выполнено, ящик и его содержимое будут удалены окончательно. 
  
Дополнительные сведения см. в следующих разделах:
  
- [Управление неактивными почтовыми ящиками в Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=286991)
    
- [Хранение на месте и хранение для судебного разбирательства](https://go.microsoft.com/fwlink/p/?LinkId=271746)
    
- [Обнаружение электронных данных на месте](https://go.microsoft.com/fwlink/p/?LinkId=271747)
    
## <a name="contacts-and-distribution-groups"></a>Контакты и группы рассылки

### <a name="offline-address-book"></a>Автономная адресная книга

Функция автономной адресной книги предоставляет моментальный снимок сведений Active Directory, доступных в глобальном списке адресов Outlook (GAL). Она кэшируется локально в Outlook таким образом, чтобы она была доступна, когда пользователь работает в автономном режиме.
  
### <a name="address-book-policies"></a>Политики адресных книг

Exchange Online поддерживает политики адресных книг. Политики адресной книги позволяют разделять пользователей на отдельные группы, чтобы предоставлять каждой из них разные представления глобального списка адресов организации. При создании политики адресной книги ей назначается глобальный список адресов, автономная адресная книга, список помещений и один или несколько списков адресов. Затем вы можете назначить политики АДРЕСНЫХ книг пользователям почтовых ящиков, предоставляя им доступ к настраиваемому глобальному спискам адресов в Outlook и Outlook в Интернете. Администраторы могут настроить политики адресной книги с помощью удаленного сеанса Windows PowerShell. Чтобы узнать больше о политиках адресной книги, ознакомьтесь со статьей " [адресные книги в Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=394203)".
  
### <a name="address-lists"></a>Списки адресов

Exchange Online поддерживает настройку списков адресов и глобальных списков адресов. Глобальный список адресов — это каталог всей организации всех пользователей с включенной поддержкой почты, групп рассылки и внешних контактов. Администраторы могут скрывать пользователей, группы рассылки и контакты из глобального списка адресов с помощью средства синхронизации каталогов или удаленной оболочки Windows PowerShell.
  
### <a name="hierarchical-address-books"></a>Иерархические адресные книги

 Иерархическая адресная книга позволяет конечным пользователям искать получателей в своей организации Exchange с помощью организационной иерархии. Администраторы могут располагать контакты в адресной книге не в алфавитном порядке, а по старшинству и в соответствии с рангом. 
  
### <a name="distribution-groups-global"></a>Группы рассылки (глобальные)

Группа рассылки (или список рассылки) — это набор пользователей, контактов и других групп рассылки, которые будут доступны всем пользователям в организации. Пользователи отправляют электронную почту на псевдоним группы рассылки для отправки сообщений всем пользователям в группе. Группы рассылки аналогичны личным группам рассылки, которые можно создать в Outlook, но списки их участников доступны в пределах всех организации. Администраторы создают группы рассылки в Центре администрирования Exchange. Группы также могут синхронизироваться с Exchange Online через локальный каталог Active Directory. Они отображаются в глобальном списке адресов в Outlook. Exchange Online поддерживает расширенные возможности групп рассылок, включая описанные ниже:
  
- **Ограниченные группы рассылки** По умолчанию, любой пользователь может отправить сообщение в любую группу рассылки. Администраторы могут изменить разрешения для определенных пользователей, чтобы разрешить отправлять электронную почту для определенной группы только им, например, чтобы воспрепятствовать ненадлежащему использованию больших списков рассылки. Администраторы также могут заблокировать внешние источники, запрещая им отправлять электронную почту с использованием групп рассылки в целях предотвращения нежелательных рассылок. Для групп рассылки, синхронизированных из локального каталога Active Directory с помощью средства синхронизации каталогов, атрибуты ограничения автоматически синхронизируются в облаке. Подробную информацию см. в статье [Управление группами рассылки](https://technet.microsoft.com/library/mt577270%28v=exchg.160%29.aspx).
    
- **Динамические группы рассылки** Списки членов динамических групп рассылки (известных также как динамические списки рассылки или списки рассылки, основанные на запросах) определяются при каждой отправке сообщения в группу. Это действие выполняется на основе заданных фильтров и условий. Группы управляются в Exchange Online через удаленную консоль Windows PowerShell. Подробную информацию о динамических группах рассылки см. в статье [Управление динамическими группами рассылки](https://technet.microsoft.com/library/bb123722%28v=exchg.160%29.aspx).
    
    > [!IMPORTANT]
    > Средство синхронизации каталогов для Microsoft Office 365 игнорирует динамические группы рассылки в локальном каталоге Active Directory и не выполняет их синхронизацию в Exchange Online. Организации, которые используют средства синхронизации службы каталогов, должны использовать соглашение об именах, которое избегает конфликтов между обычными группами рассылки, которые управляются локально, и динамическими группами рассылки, которые управляются в Exchange Online. 
  
- **Модерируемые группы рассылки** Администраторы могут выбрать модератора для управления потоком сообщений в группу рассылки. В модерируемые группы рассылки электронную почту может отправлять кто угодно, но до того, как она будет доставлена членам группы, модератор должен проверить и утвердить ее. Дополнительную информацию о модерировании см. в разделе "Утверждение сообщений" статьи [Управление группами рассылки](https://technet.microsoft.com/library/mt577270%28v=exchg.160%29.aspx).
    
- **Группы рассылки, предусматривающие самообслуживание**. Администраторы могут предоставить возможность пользователям управлять членством в группах рассылки через веб-интерфейс. Пользователям можно разрешить создавать, удалять, покидать группы рассылки или вступать в них. Эти возможности есть по умолчанию у всех пользователей Exchange Online. Администраторы могут отменить их, предоставив управление группами рассылки ИТ-отделу. Они также могут создать политики именования для стандартизации имен групп рассылки, которые создают пользователи. Например, администраторы могут добавить определенный префикс или суффикс к имени создаваемой группы рассылки или заблокировать использование определенных слов в имени группы. 
    
    > [!IMPORTANT]
    > Возможности самообслуживания недоступны для групп рассылки, синхронизируемых из локального каталога Active Directory в Exchange Online. Организации, которые используют средства синхронизации службы каталогов, должны использовать соглашение об именах, которое избегает конфликтов между обычными группами рассылки, которые управляются локально, и динамическими группами рассылки, которые управляются в облаке. 
  
### <a name="external-contacts-global"></a>Внешние контакты (глобальный список)

Внешний контакт — это запись, содержащая сведения о человеке, который работает за пределами указанной организации. Они аналогичны личным контактам, которые можно создать в Outlook, но доступны в пределах всех организации. Администраторы создают внешние контакты с помощью удаленного сеанса Windows PowerShell или Центра администрирования Exchange. Контакты также могут синхронизироваться с Exchange Online через локальный каталог Active Directory. Они отображаются в глобальном списке адресов в Outlook.
  
Дополнительную информацию о внешних контактах см. в статье [Создание связи организации в Exchange Online](https://technet.microsoft.com/library/jj916671%28v=exchg.150%29.aspx).
  
## <a name="calendar-and-scheduling"></a>Календарь и расписание

### <a name="resource-mailboxes"></a>Почтовые ящики ресурса

Почтовые ящики ресурсов (например, конференц-залов и оборудования) служат для представления конференц-залов или иных ресурсов организации. Пользователи могут резервировать комнаты или ресурсы, добавляя псевдоним электронной почты ресурса для приглашений на собрания в Outlook или Outlook в Интернете. Конференц-залов и ресурсы отображаются в глобальном списке адресов в Outlook и Outlook в Интернете.
  
Администраторы создают почтовые ящики ресурсов, используя центр администрирования Exchange или удаленный сеанс Windows PowerShell. Почтовые ящики также могут синхронизироваться с Exchange Online через локальный каталог Active Directory.
  
Дополнительные сведения о почтовых ящиках ресурсов см. в разделе
  
- [Создание почтовых ящиков помещений и управление ими](https://go.microsoft.com/fwlink/?LinkId=717533&amp;clcid=0x409)
    
- [Управление почтовыми ящиками оборудования](https://go.microsoft.com/fwlink/?LinkId=717534)
    
### <a name="conference-room-management"></a>Управление конференц-залами

Служба Exchange Online содержит помощник по резервированию ресурсов, который автоматизирует бронирование залов и других ресурсов. Почтовый ящик ресурса с настроенным RBA принимает, отклоняет или подтверждает приглашения на собрания от организаторов собраний на основе календаря доступности ресурса. 
  
Администраторы могут настраивать автоматические ответы для конференц-зала и настраивать политики резервирования в Outlook в Интернете. Такая политика указывает, кто может бронировать ресурс, когда он может быть забронирован, какие сведения будут отображены в календаре ресурса, а также допустимый процент конфликтов расписаний. Администраторы могут отключить помощник по резервированию ресурсов и назначить конкретным пользователям возможность вручную контролировать приглашения на собрания для залов.
  
Администраторы управляют параметрами RBA с помощью удаленной консоли Windows PowerShell.
  
### <a name="out-of-office-replies"></a>Ответы об отсутствии на работе

Сообщения об отсутствии — это автоматические ответы на входящие сообщения, которые Exchange Online отправляет от имени пользователя. Пользователи могут планировать сообщения об отсутствии заранее, с определенным временем начала и завершения, а также могут настраивать отдельные сообщения об отсутствии для внутренних и внешних получателей. Они также могут задавать сообщения об отсутствии с мобильных устройств, которые поддерживают данную функцию в Exchange ActiveSync. Отслеживание нежелательной электронной почты и списков рассылки в Exchange Online предотвращает отправку внешних сообщений об отсутствии в большие списки рассылок и потенциально злонамеренным пользователям. Кроме того, администраторы могут запретить пользователям отправку сообщений об отсутствии для внешних пользователей с использованием удаленной оболочки Windows PowerShell.
  
### <a name="calendar-sharing"></a>Общий доступ к календарю

Пользователи могут опубликовать свой личный календарь одним из двух способов:
  
- **Федеративный доступ к календарю** Под федерацией понимается базовая инфраструктура отношений доверия, поддерживающая федеративный общий доступ  простой способ для пользователей Exchange обмениваться сведениями о занятости на основе календаря и контактными данными с получателями во внешних федеративных организациях. Сюда включаются организации, использующие Exchange Online, а также организации с локальными системами Exchange Server 2010 или Exchange Server 2013. Администраторам Exchange Online не требуется настраивать отношения доверия с шлюзом Microsoft Federation Gateway, так как этот уровень доверия предварительно настроен для всех клиентов Exchange Online при создании службы Майкрософт. Политика общего доступа по умолчанию позволяет пользователям отправлять приглашения на общий доступ к календарю из Outlook в Интернете или Outlook 2010. Администраторы используют удаленную консоль Windows PowerShell, чтобы отключить эту политику, а также для настройки уровня данных, к которым пользователи могут открывать общий доступ в календаре. Администраторы также могут создать связь с другой федеративной организацией, которая обеспечивает требуемый уровень сведений о занятости для каждого пользователя без необходимости отправки приглашений на доступ отдельным пользователям. В рамках политик общего доступа, определяемых администратором, и связей организаций пользователи могут отдельно ограничить общий доступ. 
    
- **Доступ к календарю через Интернет** Служба Exchange Online позволяет публиковать календари в формате iCal для анонимного доступа внутри или за пределами организации. Получатели могут использовать Exchange, другую платформу или просто веб-браузер. Пользователи Exchange Online также могут подписаться на календари, опубликованные другими пользователями в Интернет-адресах с помощью iCal. Это отличается от федеративного доступа к календарю, который настраивается администратором и обеспечивает совместный доступ к данным о занятости между организациями. Пользователи не могут публиковать данные календаря в формате iCal до тех пор, пока администратор не настроил и не применит его к политике общего доступа. Администраторы могут отключить публикацию и подписку на iCal для пользователей в организации с помощью удаленной оболочки Windows PowerShell.
    
Дополнительные сведения о федеративном общем доступе см. в разделе [Общий доступ в Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=271774).
  
### <a name="outlook-2010-room-finder"></a>Средство поиска помещений Outlook 2010

Exchange Online поддерживает поиск помещений в Outlook 2010, который упорядочивает помещения в списки (например, список под названием "Помещения в корпусе 5") для упрощения поиска расположенных поблизости помещений при планировании собрания. Для вхождения в список группа рассылки должна быть специально отмечена одним из двух методов: 
  
- Новый список можно создать с помощью удаленной консоли Windows PowerShell. 
    
- Любая группа рассылки, содержащая только помещения, может быть преобразована в список помещений с помощью удаленной оболочки Windows PowerShell.
    
## <a name="feature-availability"></a>Доступность функций

Просмотреть сведения о доступности функций в планах, отдельных и локальных решениях можно в статье [Exchange Online Service Description](exchange-online-service-description.md).
  