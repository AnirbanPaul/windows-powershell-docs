---
author: brianlic-msft
description: 
external help file: MultiPoint.dll-Help.xml
keywords: powershell, cmdlet
manager: alanth
ms.date: 2016-12-20
ms.prod: powershell
ms.technology: powershell
ms.topic: reference
online version: 
schema: 2.0.0
title: Close-WmsApp
ms.assetid: 050C6E96-D91B-4020-B752-859BEA975416
---

# Close-WmsApp

## SYNOPSIS
Closes an application.

## SYNTAX

```
Close-WmsApp [-SessionId] <UInt32> [-ProcessId] <UInt32> [-WindowId] <UInt64> [-CreateTime] <UInt64>
 [-Server <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Close-WmsApp** cmdlet closes the specified application using the specified process ID and window ID.
The cmdlet first attempts to close the application gracefully.
If the application does not close gracefully, the cmdlet forces the application to close.

## EXAMPLES

### Example 1: Close an application
```
PS C:\>Close-WmsApp -SessionId 3 -ProcessId 852 -WindowId 65854 -CreateTime 45689009809823
```

This command closes the application running on session 3 with the process ID 852 and window ID 65854.

Use Get-WmsApp to get a list of applications along with their process IDs and window IDs.

## PARAMETERS

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreateTime
Specifies the process creation time.

```yaml
Type: UInt64
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ProcessId
Specifies the ID of the process to close.

```yaml
Type: UInt32
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Server
Specifies the fully qualified host name of the MultiPoint Server that is the target of the command.
The default is localhost.

```yaml
Type: String
Parameter Sets: (All)
Aliases: ComputerName

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SessionId
Specifies the ID of the session.

```yaml
Type: UInt32
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WindowId
Specifies the ID of the window.

```yaml
Type: UInt64
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

###  
None.

## OUTPUTS

###  
None.

## NOTES

## RELATED LINKS

[Get-WmsApp](./Get-WmsApp.md)

[Open-WmsApp](./Open-WmsApp.md)
