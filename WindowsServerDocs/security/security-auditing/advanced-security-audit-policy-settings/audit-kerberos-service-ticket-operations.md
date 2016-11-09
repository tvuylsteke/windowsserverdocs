---
title: Audit Kerberos Service Ticket Operations
description: "Windows Server Security"
ms.custom: na
ms.prod: windows-server-threshold
ms.reviewer: na
ms.suite: na
ms.technology: security-auditing
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 7845e359-6d3f-4853-b0be-a897c36eafa5
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/12/2016
---
# Audit Kerberos Service Ticket Operations

>Applies To: Windows Server&reg; 2016, Windows Server&reg; 2012 R2, Windows Server&reg; 2012

This topic for the IT professional describes the Advanced Security Audit policy setting, **Audit Kerberos Service Ticket Operations**, which determines whether the operating system generates security audit events for Kerberos service ticket requests.

Events are generated every time Kerberos is used to authenticate a user who wants to access a protected network resource. Kerberos service ticket operation audit events can be used to track user activity.

Event volume:

-   High on a domain controller that is in a Key Distribution Center (KDC)

-   Low on domain members

Default: Not configured

If this policy setting is configured, the following events appear on computers running the supported versions of the Windows operating system as designated in the **Applies To** list at the beginning of this topic, in addition to Windows Server 2008 and Windows Vista.

|Event ID|Event message|
|------|---------|
|4769|A Kerberos service ticket was requested.|
|4770|A Kerberos service ticket was renewed.|

## Related resource
[Advanced Security Audit Policy Settings](../advanced-security-audit-policy-settings.md)

