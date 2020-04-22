---
title: Службы голосовых сообщений
ms.author: sharik
author: skjerland
manager: mnirkhe
audience: ITPro
ms.topic: reference
f1_keywords:
- office-365-voice-message-services
ms.service: o365-administration
localization_priority: Normal
ms.custom: Adm_ServiceDesc
ms.assetid: a02af6e2-75c2-4e83-843e-77241072068e
ms.openlocfilehash: f1bf261e002eb7c8a637266c3b243ad728c63be3
ms.sourcegitcommit: 7a68dc894dde0d06fab014c56914a78aa8cda847
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43640317"
---
# <a name="voice-message-services"></a><span data-ttu-id="d3535-102">Службы голосовых сообщений</span><span class="sxs-lookup"><span data-stu-id="d3535-102">Voice message services</span></span>

## <a name="voice-mail"></a><span data-ttu-id="d3535-103">Голосовая почта</span><span class="sxs-lookup"><span data-stu-id="d3535-103">Voice mail</span></span>

<span data-ttu-id="d3535-104">Microsoft Exchange Online предлагает услуги размещенной голосовой почты, которые включают в себя следующее.</span><span class="sxs-lookup"><span data-stu-id="d3535-104">Microsoft Exchange Online offers hosted voice mail services, which provide:</span></span>
  
- <span data-ttu-id="d3535-105">Автоответчик (голосовая почта)</span><span class="sxs-lookup"><span data-stu-id="d3535-105">Call answering (voice mail)</span></span>
    
- <span data-ttu-id="d3535-106">Удаленный доступ к Exchange (голосовой доступ к Outlook)</span><span class="sxs-lookup"><span data-stu-id="d3535-106">Dial-in user interface to Exchange (Outlook Voice Access)</span></span>
    
- <span data-ttu-id="d3535-107">Удаленный доступ для вызывающих абонентов (автосекретарь)</span><span class="sxs-lookup"><span data-stu-id="d3535-107">Dial-in interface for callers (auto attendant)</span></span>
    
<span data-ttu-id="d3535-108">Размещенные службы обмена голосовыми сообщениями позволяют компании подключить свою локальную телефонную систему к службам голосовой почты, предоставляемым Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="d3535-108">Hosted voice messaging services allow a company to connect its on-premises phone system to voice mail services provided by Exchange Online.</span></span> <span data-ttu-id="d3535-109">Сообщения голосовой почты записываются и хранятся в инфраструктуре Exchange Online, что позволяет пользователям получать доступ к голосовым сообщениям из Outlook, Outlook в Интернете или на мобильных телефонах.</span><span class="sxs-lookup"><span data-stu-id="d3535-109">Voice mail messages are recorded and stored in the Exchange Online infrastructure, allowing users to access their voice messages from Outlook, Outlook on the web, or mobile phones.</span></span> <span data-ttu-id="d3535-110">Для всех телефонных соединений с Exchange Online требуются протоколы VoIP.</span><span class="sxs-lookup"><span data-stu-id="d3535-110">All telephony connections to Exchange Online require voice-over-IP (VoIP) protocols.</span></span> <span data-ttu-id="d3535-111">Администраторы могут подключить локальные УАТС на базе протокола IP или телефонные системы УАТС к Exchange Online с помощью шлюзов VoIP и пограничных контроллеров сеансов.</span><span class="sxs-lookup"><span data-stu-id="d3535-111">Administrators can connect on-premises IP PBXs or PBX phone systems using VoIP media gateways and session border controllers (SBCs) to Exchange Online.</span></span> <span data-ttu-id="d3535-112">Шлюз VoIP не требуется, если клиент развернул УАТС на базе протокола IP или если УАТС непосредственно поддерживает VoIP и взаимодействует со службами обмена голосовыми сообщениями Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3535-112">A VoIP media gateway is not required if the customer has deployed an IP PBX or if a PBX supports VoIP directly and is interoperable with Exchange voice messaging services.</span></span> <span data-ttu-id="d3535-113">Пограничные контроллеры сеансов размещаются по периметру сети заказчика для подключения локальной телефонной сети и защищают коммуникации (и клиентскую сеть) от прослушивания и вмешательства.</span><span class="sxs-lookup"><span data-stu-id="d3535-113">SBCs are deployed in the perimeter of the customer network to connect an on-premises telephony network and help secure the communications (and the customer network) against eavesdropping and intrusion.</span></span> <span data-ttu-id="d3535-114">Также поддерживается взаимодействие с голосовыми возможностями Microsoft Lync Server 2010 и 2013.</span><span class="sxs-lookup"><span data-stu-id="d3535-114">Interoperability with the voice capabilities of Microsoft Lync Server 2010 and 2013 is also supported.</span></span>
  
<span data-ttu-id="d3535-115">Функции служб обмена голосовыми сообщениями, доступные в Exchange Online, аналогичны тем, которые предлагаются на локальном сервере Exchange Server 2016.</span><span class="sxs-lookup"><span data-stu-id="d3535-115">The voice messaging services features available in Exchange Online are similar to those offered in on-premises Exchange Server 2016.</span></span> <span data-ttu-id="d3535-116">Они включают:</span><span class="sxs-lookup"><span data-stu-id="d3535-116">These include:</span></span>
  
- <span data-ttu-id="d3535-117">Проигрывание на телефоне из Outlook и Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="d3535-117">Play on phone from Outlook and Outlook on the web.</span></span>
    
- <span data-ttu-id="d3535-118">Уведомления о пропущенных вызовах.</span><span class="sxs-lookup"><span data-stu-id="d3535-118">Missed call notifications.</span></span>
    
- <span data-ttu-id="d3535-119">Идентификатор звонящего (используется информация в глобальном списке адресов, личные контакты пользователя, пользовательские папки контактов и контакты из внешних социальных сетей).</span><span class="sxs-lookup"><span data-stu-id="d3535-119">Caller ID (using information in the Global Address List, users' personal contacts, custom Contacts folder, and contacts from external social networks).</span></span>
    
- <span data-ttu-id="d3535-120">Сброс ПИН-кода голосовой почты из Outlook в Интернете и Outlook (см. [Сброс ПИН-кода голосовой почты](https://go.microsoft.com/fwlink/p/?LinkId=286328)).</span><span class="sxs-lookup"><span data-stu-id="d3535-120">Voice mail PIN reset from Outlook on the web and Outlook (see [Reset a Voice Mail PIN](https://go.microsoft.com/fwlink/p/?LinkId=286328)).</span></span>
    
- <span data-ttu-id="d3535-121">Индикатор ожидающего сообщения (дополнительные сведения см. в статье об [индикаторе ожидающих сообщений в Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=271794)).</span><span class="sxs-lookup"><span data-stu-id="d3535-121">Message Waiting Indicator (see [MWI in Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=271794) for details).</span></span> 
    
- <span data-ttu-id="d3535-122">Правила автоответчика (см. раздел [Разрешить пользователям голосовой почты пересылать звонки](https://go.microsoft.com/fwlink/p/?LinkId=271795) для получения дополнительных сведений).</span><span class="sxs-lookup"><span data-stu-id="d3535-122">Call answering rules (see [Allow voice mail users to forward calls](https://go.microsoft.com/fwlink/p/?LinkId=271795) for details).</span></span>
    
- <span data-ttu-id="d3535-123">Защищенная голосовая почта в Exchange Online (Дополнительные сведения см. [в статье Защита голосовой почты в Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=271796) ).</span><span class="sxs-lookup"><span data-stu-id="d3535-123">Protected voice mail in Exchange Online (see [Protect voice mail in Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=271796) for details).</span></span>
    
- <span data-ttu-id="d3535-124">Просмотр голосовой почты (см. раздел [Разрешить пользователям просмотр записи голосовой почты](https://go.microsoft.com/fwlink/p/?LinkId=271797) для списка поддерживаемых языков).</span><span class="sxs-lookup"><span data-stu-id="d3535-124">Voice mail preview (see [Allow users to see a voice mail transcript](https://go.microsoft.com/fwlink/p/?LinkId=271797) for a list of supported languages).</span></span>
    
- <span data-ttu-id="d3535-125">Голосовой доступ к электронной и голосовой почте, календарю, личным контактам и личным группам контактов.</span><span class="sxs-lookup"><span data-stu-id="d3535-125">Speech access to email, voice mail, calendar, personal contacts, and personal contact groups.</span></span>
    
- <span data-ttu-id="d3535-126">Поиск по каталогу с помощью голосового доступа к Outlook или автосекретаря.</span><span class="sxs-lookup"><span data-stu-id="d3535-126">Directory search through Outlook Voice Access or an auto attendant.</span></span>
    
- <span data-ttu-id="d3535-127">Администраторы настраивают и управляют совместимостью служб обмена голосовыми сообщениями с помощью Центра администрирования Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3535-127">Administrators configure and manage voice messaging services interoperability by using the Exchange admin center (EAC).</span></span>
    
<span data-ttu-id="d3535-128">Дополнительные сведения о функциях голосовой почты вы найдете [в статье Служба голосовой почты в Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=271798).</span><span class="sxs-lookup"><span data-stu-id="d3535-128">For more information about voice mail features, see [Voice mail in Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=271798).</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="d3535-129">Функция автоматического распознавания речи (ASR) недоступна во время навигации по меню или поиска по каталогу для пользователей голосового доступа к Outlook или пользователей автосекретаря, использующих голосовые команды.</span><span class="sxs-lookup"><span data-stu-id="d3535-129">The Automatic Speech Recognition (ASR) feature isn't available in menu navigation or directory search for Outlook Voice Access users or auto attendant callers using voice commands.</span></span> 
>
> <span data-ttu-id="d3535-130">Клиент должен предоставить телефонное подключение из телефонной сети общего пользования (PSTN), используя шлюз VoIP и УАТС, IP-УАТС или Skype для бизнеса Server 2015.</span><span class="sxs-lookup"><span data-stu-id="d3535-130">The customer must provide a telephony connection from the public switched telephone network (PSTN) using a VoIP gateway and PBX, IP PBX, or Skype for Business Server 2015.</span></span> 
>
> <span data-ttu-id="d3535-p103">Клиент должен предоставить локальные устройства пограничных контроллеров сеансов (SBC) и обеспечить правильную настройку SBC для подключения к службам голосовой почты в Интернете. Сюда входит настройка соответствующего уровня безопасности с использованием сертификатов, общедоступных и частных интерфейсов IP и подключением соответствующих портов TCP через их локальные брандмауэры.</span><span class="sxs-lookup"><span data-stu-id="d3535-p103">The customer must provide the on-premises SBC hardware devices and ensure that the SBCs are correctly configured to connect to the online voice mail services. This includes configuring the appropriate level of security by using certificates and public and private IP interfaces and by enabling the correct TCP ports through their on-premises firewalls.</span></span> 
>
> <span data-ttu-id="d3535-133">Размещенная Голосовая почта доступна только для подписчиков Exchange Online (план 2) и Office 365 для предприятий E3.</span><span class="sxs-lookup"><span data-stu-id="d3535-133">Hosted voice mail is available only to Exchange Online Plan 2 and Office 365 Enterprise E3 subscribers.</span></span> 
  
## <a name="third-party-voice-mail-interoperability"></a><span data-ttu-id="d3535-134">Взаимодействие со сторонней голосовой почтой</span><span class="sxs-lookup"><span data-stu-id="d3535-134">Third-party voice mail interoperability</span></span>

<span data-ttu-id="d3535-p104">Локальные системы голосовой почты от сторонних провайдеров могут взаимодействовать с Exchange Online, если они способны пересылать голосовые сообщения через SMTP, или если они поддерживают службы Microsoft Exchange Web Services. Если система голосовой почты изначально не поддерживает переадресацию голосовых сообщений через SMTP, сервер электронной почты может быть размещен локально и может получать сообщения из системы голосовой почты, а затем направлять их на облако используя SMTP. Так как многие сторонние системы голосовой почты используют MAPI/CDO для взаимодействия с продвинутой единой системой обмена сообщениями Exchange Server, все возможности этих систем могут быть недоступны при использовании SMTP для совместимости с Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="d3535-p104">On-premises voice mail solutions from third-party providers can interoperate with Exchange Online if they can forward voice messages through SMTP or if they support Microsoft Exchange Web Services. If the voice mail system does not natively support forwarding voice messages through SMTP, an email server can be kept on-premises to receive messages from the voice mail system and then forward them to the cloud using SMTP. Because many third-party voice mail systems use MAPI/CDO to interoperate with Exchange Server for advanced UM features, the full capabilities of these systems may not be available when SMTP is used for interoperability with Exchange Online.</span></span>
  
> [!NOTE]
> <span data-ttu-id="d3535-138">Поддержка единой системы обмена сообщениями Exchange Online единой системы обмена сообщениями с непосредственными подключениями от пользователей, истечений с помощью прямых подключений, будет завершаться 2018 июля</span><span class="sxs-lookup"><span data-stu-id="d3535-138">Exchange Online UM support for third-party PBX systems via direct connections from customer operated SBCs will end in July 2018.</span></span> <span data-ttu-id="d3535-139">Дополнительную информацию можно узнать в статье прекращение [поддержки пограничных контроллеров сеансов в единой системе обмена сообщениями Exchange Online](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/Discontinuation-of-support-for-Session-Border-Controllers-in/ba-p/607117) .</span><span class="sxs-lookup"><span data-stu-id="d3535-139">Please see [Discontinuation of support for Session Border Controllers in Exchange Online Unified Messaging](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/Discontinuation-of-support-for-Session-Border-Controllers-in/ba-p/607117) for more information.</span></span> 
  
## <a name="skype-for-business-integration"></a><span data-ttu-id="d3535-140">Интеграция Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="d3535-140">Skype for Business integration</span></span>

<span data-ttu-id="d3535-141">Организации могут приобрести Skype для бизнеса Online в качестве автономной службы или в составе Microsoft Office 365.</span><span class="sxs-lookup"><span data-stu-id="d3535-141">Organizations can purchase Skype for Business Online as a standalone service or as part of Microsoft Office 365.</span></span> <span data-ttu-id="d3535-142">Локальная среда Skype для бизнеса 2015 также поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3535-142">Skype for Business 2015 on-premises is also supported.</span></span> <span data-ttu-id="d3535-143">Дополнительные сведения о Skype для бизнеса Online см. в [описании службы Skype для бизнеса Online](../skype-for-business-online-service-description/skype-for-business-online-service-description.md).</span><span class="sxs-lookup"><span data-stu-id="d3535-143">To learn more about Skype for Business Online, see [Skype for Business Online service description](../skype-for-business-online-service-description/skype-for-business-online-service-description.md).</span></span>
  
## <a name="feature-availability"></a><span data-ttu-id="d3535-144">Доступность функций</span><span class="sxs-lookup"><span data-stu-id="d3535-144">Feature availability</span></span>

<span data-ttu-id="d3535-145">Просмотреть сведения о доступности функций в планах, отдельных и локальных решениях можно в статье [Exchange Online Service Description](exchange-online-service-description.md).</span><span class="sxs-lookup"><span data-stu-id="d3535-145">To view feature availability across plans, standalone options, and on-premises solutions, see [Exchange Online service description](exchange-online-service-description.md).</span></span>
  

