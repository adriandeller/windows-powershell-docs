---
external help file: OnlineBackup_Cmdlets.xml
online version: 
schema: 2.0.0
ms.reviewer:
ms.author: v-anbarr
author: andreabarr
ms.assetid: 647F4668-4E36-47EA-BC59-BAC6F01DACE3
manager: dansimp
---

# Get-OBNotification

## SYNOPSIS
Gets array of OBNotification objects which are applicable for the server.

## SYNTAX

```
Get-OBNotification
```

## DESCRIPTION
The **Get-OBNotification** cmdlet gets the array of OBNotification\[\] objects for the server.

The OBNotification\[\] object contains the following details regarding the notification. 
1) Category of Notification 
2) Type of Notification 
3) Time of generation of Notification 
4) ErrorCodes for Long and short description 
5) **ErrorMessage** parameters.

If a server is unregistered with the mob_name_1 service, the event log is not cleared.
This can result in notifications generated by a previous registration being returning in this array if a server is re-registered with mob_name_1.

However, if the mob_agent is uninstalled completely from the server the event logs are deleted.

ps_mob_user_group_remark

## EXAMPLES

### EXAMPLE 1
```
PS C:\>Get-OBNotification
```

This example gets notifications for the server.

## PARAMETERS

## INPUTS

### None

## OUTPUTS

### Microsoft.Internal.CloudBackup.Commands.OBNotification[]

## NOTES

## RELATED LINKS

[00000000-0000-0000-0000-000000000000](00000000-0000-0000-0000-000000000000)

