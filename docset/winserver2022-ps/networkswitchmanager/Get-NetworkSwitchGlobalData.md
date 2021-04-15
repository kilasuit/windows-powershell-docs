---
author: Kateyanne
description: Use this topic to help manage Windows and Windows Server technologies with Windows PowerShell.
external help file: NetworkSwitchGlobalSettingData-help.xml
manager: jasgro
Module Name: NetworkSwitchManager
ms.author: v-kaunu
ms.date: 12/20/2016
ms.mktglfcycl: manage
ms.prod: w10
ms.reviewer: 
ms.sitesec: library
ms.technology: 
ms.topic: reference
online version: https://docs.microsoft.com/powershell/module/networkswitchmanager/get-networkswitchglobaldata?view=windowsserver2022-ps&wt.mc_id=ps-gethelp
schema: 2.0.0
title: Get-NetworkSwitchGlobalData
---

# Get-NetworkSwitchGlobalData

## SYNOPSIS
Gets global data of a network switch.

## SYNTAX

```
Get-NetworkSwitchGlobalData [-CimSession] <CimSession> [<CommonParameters>]
```

## DESCRIPTION
The **Get-NetworkSwitchGlobalData** cmdlet gets global data of a network switch.

## EXAMPLES

### Example 1: Get global data
```
PS C:\>$Session = New-CimSession -ComputerName "NetworkSwitch08"
PS C:\> Get-NetworkSwitchGlobalData -CimSession $Session
```

The first command creates a **CimSession** for a network switch, and then stores it in the **$Session** variable.
For more information about **CimSession** objects, type `Get-Help New-CimSession`.

The second command gets global data for the network switch NetworkSwitch08 by using the **$Session** object.

## PARAMETERS

### -CimSession
Specifies the **CimSession** that this cmdlet uses to connect to the network switch.
For more information about **CimSession** objects, type `Get-Help New-CimSession`.

```yaml
Type: CimSession
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](https://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### CimInstance
This cmdlet returns the **globalData** of the network switch as **CimInstance** object.

## NOTES

## RELATED LINKS
