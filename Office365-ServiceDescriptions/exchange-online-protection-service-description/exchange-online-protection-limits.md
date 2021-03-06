---
title: Ограничения Exchange Online Protection
ms.author: office365servicedesc
author: pamelaar
audience: ITPro
ms.topic: reference
f1_keywords:
- exchange-online-protection-limits
ms.service: o365-administration
localization_priority: Normal
ms.custom: Adm_ServiceDesc
ms.assetid: f866fe3b-a183-4e6d-abd9-bbec0a0c7fae
description: В настоящее время существуют следующие ограничения для Exchange Online Protection. Эти пределы нельзя настраивать, если не указано иное.
ms.openlocfilehash: 555177349005c275fcbf91a1e70467ebcc25f2be
ms.sourcegitcommit: 0f17ea421190f52bf55e530e9374543fd59b8665
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2020
ms.locfileid: "48261500"
---
# <a name="exchange-online-protection-limits"></a>Ограничения Exchange Online Protection

В настоящее время существуют следующие ограничения для Exchange Online Protection. Эти пределы нельзя настраивать, если не указано иное. 
  
> [!TIP]
> Дополнительные сведения об ограничении в Exchange Online приведены в статье [Exchange Online Limits](../exchange-online-service-description/exchange-online-limits.md). Ограничения правил транспорта также применимы в случае пользователей отдельных выпусков EOP. Частота получателей и пределы скорости сообщений для Exchange Online неприменимы для отдельных клиентов EOP. 
  
- **Максимальное число** доменов — вы можете добавить до 900 доменов для каждого клиента. Дочерние домены могут быть включены в этот 900ный лимит, или если это необходимо, в составе параметра "Catch — все", сопоставлять поддомены. Дополнительные сведения см в разделе [Manage обслуживаемые домены в EOP](https://go.microsoft.com/fwlink/p/?LinkId=282239).

- **Предельное число удаленных доменов** — вы можете добавить до 200 удаленных доменов для каждого клиента.
    
- **Ограничение размера сообщения** — максимальный размер сообщения для отдельных пользователей EOP, включая вложения, составляет 150 МБ. 
    
- **Количество отправленных исходящих сообщений** : количество исходящих сообщений, отправляемых через EOP, достаточно велико для обеспечения обычной связи с электронной почтой, которая не считается нежелательной. Если вам нужно выполнять массовые рассылки электронной почты в коммерческих целях вместо отправки сообщений через EOP, мы рекомендуем вам обратиться к стороннему поставщику услуг электронной почты или отправлять их через локальные почтовые серверы. 
    
- **Предельное число получателей** (до тех пор, пока узел-отправитель может разделить сообщение на "фрагменты" менее 500 получателей, не определено ни одного явного ограничения. Однако каждый "блок" фактически обрабатывается как новое сообщение. Слишком много сообщений за короткое время, сообщения от узла с плохой репутацией или сообщения с сомнительным содержимым могут регулироваться или блокироваться. 
    
- **Ограничение списка разрешенных или заблокированных** IP-адресов — при настройке списка РАЗРЕШЕНных IP-адресов или списка ЗАБЛОКИРОВАНных IP-адресов в фильтре подключения можно указать не более 1273 записей, где запись является одним IP-адресом или ДИАПАЗОНОМ CIDR IP-адресов от/24 до/32. 
    
- **Лимит расхода для сообщений** — сообщения в РБП будут храниться в очередях в течение 24 часов. Попытки повторной отправки сообщений зависят от типа ошибки, полученной от почтовой системы получателя. Повторные попытки выполняются каждые 15 минут. 
    
- Срок **хранения в карантине нежелательной почты** по умолчанию сообщения, отправляемые в карантин, хранятся в течение 30 дней. Администраторы снизить это значение с помощью политик фильтрации содержимого. 
    
- **Уведомления карантина нежелательной почты пользователя** по умолчанию при включении уведомления о нежелательной почте для конечных пользователей отправляются через каждые 3 дня. Этот срок можно изменить, указав от 1 до 15 дней. 
    
- В разделе "отчеты и отслеживание сообщений трассировки сообщений и задержка" в отчетах и [трассировке сообщений в службе Exchange Online Protection](https://go.microsoft.com/fwlink/?LinkId=394248)доступны **ограниченные** отчеты и сведения о них.
    
### <a name="limits-across-eop-options"></a>Ограничения на параметры EOP

| Компонент | Отдельный выпуск EOP | Функции EOP в Exchange Online | Клиентская лицензия Exchange Enterprise CAL со службами |
|:-----|:-----|:-----|:-----|
|Ограничения домена  <br/> |900  <br/> |900  <br/> |900  <br/> |
|Ограничения для удаленных доменов  <br/> |200  <br/> |200  <br/> |200  <br/> |
|Ограничение на размер сообщений (учитывая вложения)  <br/> |150 МБ  <br/> |150 МБ  <br/> |150 МБ  <br/> |
|Ограничение числа получателей  <br/> |См. раздел "Максимальное число получателей" выше  <br/> |500 получателей при отправке с размещенного почтового ящика. Другие сценарии см. в разделе "Максимальное число получателей" выше  <br/> |См. раздел "Максимальное число получателей" выше  <br/> |
|Максимальное количество надежных отправителей  <br/> |1024 записи  <br/> |1024 записи  <br/> ||
|Предельное количество заблокированных отправителей для каждой политики  <br/> |1024 записи  <br/> |1024 записи  <br/> ||
|Ограничение на списки разрешенных или заблокированных IP-адресов  <br/> |1273 записи  <br/> |1273 записи  <br/> |1273 записи  <br/> |
|Ограничение на отложенные сообщения  <br/> |1 день, повторная попытка каждые 15 минут  <br/> |1 день, повторная попытка каждые 15 минут  <br/> |1 день, повторная попытка каждые 15 минут  <br/> |
|Период хранения нежелательных сообщений, отправленных в карантин  <br/> |30 дней по умолчанию, но их можно опустить  <br/> |30 дней по умолчанию, но их можно опустить  <br/> |30 дней по умолчанию, но их можно опустить  <br/> |
|Уведомления пользователей о нежелательных сообщениях, помещенных в карантин  <br/> |3 дня по умолчанию, можно указать от 1 до 15 дней  <br/> |3 дня по умолчанию, можно указать от 1 до 15 дней  <br/> |3 дня по умолчанию, можно указать от 1 до 15 дней  <br/> |
   

