---
title: Установка и администрирование Exchange Online
ms.author: office365servicedesc
author: pamelaar
audience: ITPro
ms.topic: reference
f1_keywords:
- exchange-online-administration-and-management
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_ServiceDesc_top
- Adm_ServiceDesc
ms.assetid: 80c07748-ac57-4b90-97dd-a2d1115009a6
description: В этой статье описываются административные элементы управления и поддержка, доступные для настройки параметров Exchange Online и поддержания среды Exchange Online в Организации, ее выполнения и текущей. Он включает сведения о средствах самостоятельного администрирования и возможностях, доступных для организаций; административные обязанности корпорации Майкрософт и обязательства производительности; а также обслуживание и обновления для продукта.
ms.openlocfilehash: 19ec50b3f502ee111de05e1a115d17f16fec3569
ms.sourcegitcommit: d2cd67e52dd646b68bfbfd8a387e70a6da140a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45133004"
---
# <a name="exchange-online-setup-and-administration"></a>Установка и администрирование Exchange Online

В этой статье описываются административные элементы управления и поддержка, доступные для настройки параметров Exchange Online и поддержания среды Exchange Online в Организации, ее выполнения и текущей. Он включает сведения о средствах самостоятельного администрирования и возможностях, доступных для организаций; административные обязанности корпорации Майкрософт и обязательства производительности; а также обслуживание и обновления для продукта.
  
## <a name="self-service-administration-tools"></a>Средства самостоятельного администрирования

Несмотря на то, что Microsoft напрямую контролирует все центры обработки данных Exchange Online и отвечает за общую производительность системы, он может управлять только частью элементов, объединяемых для предоставления общего интерфейса для пользователей. Сами организации отвечают за сетевые соединения с центрами обработки данных, глобальную сеть (WAN) и локальные сети (LAN) пользователей. Кроме того, они отвечают за устройства пользователей и их конфигурацию.Они также обеспечивают необходимое лицензирование для каждого пользователя относительно любой требующейся функции, включая возможность управления этими функциями, пока пользователю нужен доступ к этой функции.
  
Следовательно, Exchange Online предоставляет пользователям-администраторам инструменты, описанные ниже, для управления различными задачами, связанными с обменом сообщениями.
  
- [Портал Microsoft Office 365](exchange-online-setup-and-administration.md#microsoft-office-365-portal)
    
- [Центр администрирования Microsoft 365](#microsoft-365-admin-center)
    
- [Центр администрирования Exchange](exchange-online-setup-and-administration.md#exchange-admin-center)
    
- [Удаленная оболочка Windows PowerShell для Exchange Online](exchange-online-setup-and-administration.md#remote-windows-powershell-for-exchange-online)
    
### <a name="microsoft-office-365-portal"></a>Портал Microsoft Office 365

Портал Microsoft Office 365, расположенный по адресу [https://portal.office.com](https://portal.office.com), представляет из себя веб-сайт, на котором администраторы и партнеры могут приобретать службы Office 365 и управлять ими, а пользователи могут получать доступ к средствам Office 365 для совместной работы и использовать их.
  
### <a name="microsoft-365-admin-center"></a>Центр администрирования Microsoft 365

Центр администрирования Microsoft 365 — это веб-портал, с которого администратор службы каждой компании может управлять учетными записями и параметрами пользователей для каждой из служб Майкрософт, на которые они подписаны. В центре администрирования Microsoft 365 администраторы могут перейти по ссылкам в центр администрирования Exchange, где они могут управлять параметрами Exchange Online. Дополнительные сведения о том, как приступить к работе с помощью центра администрирования Microsoft 365, можно найти в следующем видео: [Введение в Office 365 корпоративный](https://go.microsoft.com/fwlink/p/?LinkId=271806).
  
### <a name="exchange-admin-center"></a>Центр администрирования Exchange

Exchange Online предоставляет единую консоль управления, которая упрощает работу и оптимизирована для управления локальными, гибридными и веб-развертываниями. В Центре администрирования Exchange администраторы могут управлять специальными параметрами Exchange.
  
Дополнительные сведения об управлении Exchange Online с помощью Центра администрирования Exchange см. в разделе [Центр администрирования Exchange](https://go.microsoft.com/fwlink/p/?LinkId=271807).
  
### <a name="remote-windows-powershell-for-exchange-online"></a>Удаленная оболочка Windows PowerShell для Exchange Online

С помощью удаленной оболочки Windows PowerShell администраторы могут подключаться к Exchange Online для выполнения задач управления, недоступных или нецелесообразных при использовании Центра администрирования Exchange. Такие задачи включают автоматизацию повторяющихся задач, извлечение данных из пользовательских отчетов, настройку политик и подключение Exchange Online к существующим процессам и инфраструктуре. Дополнительные сведения см. в статье [Подключение к Exchange Online с помощью удаленной оболочки PowerShell](https://go.microsoft.com/fwlink/p/?LinkId=308994).
  
Exchange Online использует те же командлеты оболочки Windows PowerShell, что и Exchange Server 2013, но некоторые команды и параметры недоступны, поскольку эти функции не применяются в Exchange Online. Список командлетов, которые используются с Exchange Online, см. в разделе [Командлеты Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=271808).
  
Для использования удаленной оболочки Windows PowerShell администраторам не нужно устанавливать какое-либо средство управления или миграции Exchange Server. Однако компьютеры администраторов должны работать под управлением Windows Management Framework 3.0, включающей в себя Windows PowerShell версии 3 и WinRM 3.0; а также Windows .NET Framework 4.5. Эти компоненты уже установлены на компьютере под управлением ОС Windows 8 или Windows Server 2012. Администраторы могут загружать эти компоненты на компьютеры под управлением ОС Windows 7 или Windows Server 2008 R2 вручную.
  
> [!IMPORTANT]
> Для предотвращения атак типа "отказ в обслуживании" (DoS) можно открыть не более трех подключений оболочки Windows PowerShell к организации Exchange Online. 
  
## <a name="self-service-capabilities-for-exchange-online"></a>Возможности самообслуживания для Exchange Online

Ниже приводятся важные функции, доступные для управления Exchange Online с помощью Центра администрирования Exchange, удаленной оболочки Windows PowerShell и других инструментов. С помощью этих инструментов можно контролировать и многие другие параметры, как описано в этом документе.
  
### <a name="mobile-device-security-policies-for-exchange-online"></a>Политики безопасности мобильных устройств для Exchange Online

Exchange Online поддерживает те же политики ActiveSync для мобильных устройств, что и Exchange Server 2013. Администраторы могут применять и настраивать эти политики для отдельных пользователей и групп с помощью Центра администрирования Exchange или удаленной оболочки Windows PowerShell.
  
### <a name="message-tracking-for-exchange-online"></a>Отслеживание сообщений для Exchange Online

Отслеживание сообщений с помощью функции "отчеты о доставке" описывается в следующем разделе: [функции отчетов и средства устранения неполадок](reporting-features-and-troubleshooting-tools.md).
  
### <a name="usage-reporting-for-exchange-online"></a>Использование отчетов для Exchange Online

Администраторы могут использовать удаленную оболочку Windows PowerShell для получения информации об использовании служб Exchange Online сотрудниками организации. К такой информации относятся следующие сведения.
  
- Размер почтового ящика для каждого пользователя в организации.
    
- Настраиваемые разрешения, заданные для почтовых ящиков, такие как передача прав доступа.
    
- Данные о подключении мобильных устройств, например, подключенных с помощью Exchange ActiveSync, об используемых устройствах и дате их последнего подключения.
    
Командлеты удаленной оболочки Windows PowerShell, которые начинаются с префикса "get-", могут получать данные от системы Exchange Online. Администраторы могут экспортировать эту информацию с Windows PowerShell в формате CSV для расширенного анализа или создания отчета.
  
Дополнительные сведения о командлетах Windows PowerShell, которые используются в Exchange Online, см. в разделе [Командлеты Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=271808).
  
### <a name="auditing-for-exchange-online"></a>Аудит для Exchange Online

Функция ведения журнала аудита описана в следующем разделе: [функции отчетов и средства устранения неполадок](reporting-features-and-troubleshooting-tools.md).
  
## <a name="service-and-product-upgrades-for-exchange-online"></a>Обновления служб и продуктов для Exchange Online

Клиенты Exchange Online пользуются преимуществом периодических обновлений Exchange до новейших технологий, в том числе до новых выпусков Exchange Server. Эти обновления доступны бесплатно и гарантируют, что клиенты всегда используют новейшее программное обеспечение Exchange.
  
После выпуска корпорацией Майкрософт основной версии Exchange клиенты могут обновить службы до новой версии в течение 12 месяцев.
  
## <a name="feature-availability"></a>Доступность функций

Просмотреть сведения о доступности функций в планах, отдельных и локальных решениях можно в статье [Exchange Online Service Description](exchange-online-service-description.md).
  