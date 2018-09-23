---
title: Высокая доступность и непрерывность бизнес-процессов
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/13/2018
ms.audience: ITPro
ms.topic: reference
f1_keywords:
- exchange-online-high-availability-and-business-continuity
ms.service: o365-administration
localization_priority: Normal
ms.custom: Adm_ServiceDesc
ms.assetid: 7b03465e-3b9c-4500-8956-a83377f4c2c3
description: Microsoft Exchange Online предлагает расширенную хранения и восстановления поддержка инфраструктуры электронной почты. Этот компонент включает репликации почтовых ящиков в центрах обработки данных и возможность восстановить удаленные почтовые ящики и удаленных элементов.
ms.openlocfilehash: 3f926223a278bd671fa6121b2ee59b96da1f9fe1
ms.sourcegitcommit: d6dfbaacd56c0855e12500b38acd06be16cd1560
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "24036785"
---
# <a name="high-availability-and-business-continuity"></a><span data-ttu-id="9f730-104">Высокая доступность и непрерывность бизнес-процессов</span><span class="sxs-lookup"><span data-stu-id="9f730-104">High Availability and Business Continuity</span></span>

<span data-ttu-id="9f730-p102">Microsoft Exchange Online предлагает расширенную хранения и восстановления поддержка инфраструктуры электронной почты. Этот компонент включает репликации почтовых ящиков в центрах обработки данных и возможность восстановить удаленные почтовые ящики и удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="9f730-p102">Microsoft Exchange Online offers extensive retention and recovery support for an organization's email infrastructure. This includes mailbox replication at data centers and the ability to restore deleted mailboxes and deleted items.</span></span>
  
## <a name="mailbox-replication-at-data-centers"></a><span data-ttu-id="9f730-107">Репликация почтовых ящиков в центрах обработки данных</span><span class="sxs-lookup"><span data-stu-id="9f730-107">Mailbox replication at data centers</span></span>

<span data-ttu-id="9f730-p103">Почтовые ящики Exchange Online постоянно реплицируются с созданием нескольких копий базы данных в географически распределенных центрах обработки данных Майкрософт, чтобы обеспечить возможность восстановления данных в случае локального сбоя инфраструктуры обмена сообщениями. В случае крупномасштабных сбоев инициируются процедуры по управлению непрерывностью обслуживания.</span><span class="sxs-lookup"><span data-stu-id="9f730-p103">Exchange Online mailboxes are continuously replicated to multiple database copies, in geographically dispersed Microsoft data centers, to provide data restoration capability in the event of a local messaging infrastructure failure. For large-scale failures, service continuity management procedures are initiated.</span></span>
  
<span data-ttu-id="9f730-p104">Дополнительные сведения о том, как корпорация Майкрософт защищает ваши данные, см. на странице [Центр управления безопасностью Office 365](https://go.microsoft.com/fwlink/p/?LinkId=299135). Если у вас есть план Office 365:, которым управляет 21Vianet, см. страницу [Центр 21Vianet для управления безопасностью](http://www.21vbluecloud.com/office365/trustcenter/onlineservices.mdl).</span><span class="sxs-lookup"><span data-stu-id="9f730-p104">For more information about how Microsoft protects your data, see [Office 365 Trust Center](https://go.microsoft.com/fwlink/p/?LinkId=299135). If you are using Office 365 operated by 21Vianet, see the [21Vianet Trust Center](http://www.21vbluecloud.com/office365/trustcenter/onlineservices.mdl).</span></span>
  
## <a name="deleted-mailbox-recovery"></a><span data-ttu-id="9f730-112">Восстановление удаленного почтового ящика</span><span class="sxs-lookup"><span data-stu-id="9f730-112">Deleted mailbox recovery</span></span>

<span data-ttu-id="9f730-p105">Администраторы могут удалять почтовые ящики Exchange Online, используя Центр администрирования Office 365: для удаления соответствующей учетной записи пользователя или удаления лицензии Exchange Online или используя командлет **Remove-Mailbox** в удаленном Windows PowerShell. При удалении почтового ящика Exchange Online по умолчанию хранит его и его содержимое в течение 30 дней. Через 30 дней почтовый ящик не подлежит восстановлению. Восстановленный почтовый ящик содержит все данные, которые хранились в нем на момент удаления. Администраторы могут восстановить удаленный почтовый ящик в течение периода хранения с помощью Центра администрирования Office 365:. Для восстановления удаленного почтового ящика администраторам необходимо восстановить соответствующую учетную запись пользователя Office 365: или переназначить лицензию Exchange Online для учетной записи. Дополнительные сведения см. в разделе [Удаление и восстановление почтовых ящиков пользователей в Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=286992).</span><span class="sxs-lookup"><span data-stu-id="9f730-p105">Administrators can delete Exchange Online mailboxes by using the Office 365 admin center to delete the corresponding user account or remove the Exchange Online license, or by using the **Remove-Mailbox** cmdlet in remote Windows PowerShell. When a mailbox is deleted, Exchange Online retains the mailbox and its contents for 30 days by default. After 30 days, the mailbox is not recoverable. A recovered mailbox contains all of the data stored in it at the time it was deleted. Administrators can recover a deleted mailbox within the retention period by using the Office 365 admin center. To recover a deleted mailbox, administrators have to restore the corresponding Office 365 user account or reassign an Exchange Online license to the user account. For more information, see [Delete or Restore User Mailboxes in Exchange Online](https://go.microsoft.com/fwlink/p/?LinkId=286992).</span></span>
  
## <a name="deleted-item-recovery"></a><span data-ttu-id="9f730-120">Восстановление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="9f730-120">Deleted item recovery</span></span>

<span data-ttu-id="9f730-p106">Exchange Online дает пользователям возможность восстановления элементов, удаленных из любой папки электронной почты, в том числе из папки "Удаленные". После удаления элемент хранится в пользовательской папке "Удаленные". Он остается там до удаления пользователем вручную или автоматического удаления согласно политикам хранения. Администраторы могут изменять политики хранения с помощью Центра администрирования Exchange или удаленного Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9f730-p106">Exchange Online enables users to restore items they have deleted from any email folder, including the Deleted Items folder. When an item is deleted, it's kept in a user's Deleted Items folder. It remains there until it's either manually removed by the user or automatically removed by retention policies. Administrators can customize retention policies in the EAC or by using remote Windows PowerShell.</span></span>
  
<span data-ttu-id="9f730-p107">После удаления элемента из папки "Удаленные" он хранится в папке "Элементы, подлежащие восстановлению" в течение дополнительных 14 дней, после чего безвозвратно удаляется. Тем не менее администраторы могут увеличить срок хранения до 30 дней с помощью удаленного Windows PowerShell. В течение этого периода пользователи могут восстановить элемент с помощью функции "Восстановить удаленные элементы" в Outlook Web App или Outlook. Узнайте, как [изменить срок хранения удаленных элементов](https://go.microsoft.com/fwlink/p/?LinkId=286940).</span><span class="sxs-lookup"><span data-stu-id="9f730-p107">After an item has been removed from the Deleted Items folder, it's kept in a Recoverable Items folder for an additional 14 days before being permanently removed, but administrators can increase this to a maximum of 30 days by using remote Windows PowerShell. Users can recover the item during this time period by using the Recover Deleted Items feature in Outlook Web App or Outlook. Learn how to [change the deleted item retention period](https://go.microsoft.com/fwlink/p/?LinkId=286940).</span></span>
  
<span data-ttu-id="9f730-p108">Если пользователь вручную удалил элемент из папки "Элементы, подлежащие восстановлению", администратор может восстановить элемент в течение такого же срока, используя функцию восстановления одного элемента и удаленного Windows PowerShell. По умолчанию при создании почтового ящика восстановление одного элемента включено. Узнайте, как [активировать восстановление одного элемента почтового ящика](https://go.microsoft.com/fwlink/p/?LinkID=286941).</span><span class="sxs-lookup"><span data-stu-id="9f730-p108">If a user has manually purged an item from the Recoverable Items folder, an administrator can recover the item within the same time period by using the Single Item Recovery feature with remote Windows PowerShell. By default, Single Item Recovery is enabled when a mailbox is created. To learn more, see [Enable or disable single item recovery for a mailbox](https://go.microsoft.com/fwlink/p/?LinkID=286941).</span></span>
  
<span data-ttu-id="9f730-p109">Для сохранения сообщения в папке "Элементы, подлежащие восстановлению" на период больше 30 дней организации могут внедрить политику долгосрочного хранения почты или временного хранения на месте. Дополнительные сведения см. в разделе, посвященном [удержанию почтовых ящиков на месте](https://go.microsoft.com/fwlink/p/?LinkId=271746).</span><span class="sxs-lookup"><span data-stu-id="9f730-p109">To preserve messages for longer than 30 days in the Recoverable Items folder, organizations can implement longer-term email preservation or time-based In-Place Holds. Learn more about [placing a mailbox on In-Place Hold](https://go.microsoft.com/fwlink/p/?LinkId=271746).</span></span>
  
## <a name="feature-availability"></a><span data-ttu-id="9f730-133">Доступность функций</span><span class="sxs-lookup"><span data-stu-id="9f730-133">Feature Availability</span></span>

<span data-ttu-id="9f730-134">Просмотреть функции, доступные в планах Office 365, отдельных и локальных решениях, можно в статье [Описание службы Exchange Online](exchange-online-service-description.md).</span><span class="sxs-lookup"><span data-stu-id="9f730-134">To view feature availability across Office 365 plans, standalone options, and on-premise solutions, see [Exchange Online Service Description](exchange-online-service-description.md).</span></span>
  
