---
ms.mktglfcycl: manage
ms.sitesec: library
ms.author: brianlic
author: brianlic-msft
description: Use this topic to help manage Windows and Windows Server technologies with Windows PowerShell.
external help file: Microsoft.NetworkController.Powershell.dll-Help.xml
keywords: powershell, cmdlet
manager: alanth
ms.date: 2016-12-20
ms.prod: w10
ms.technology: powershell-windows
ms.topic: reference
online version: 
schema: 2.0.0
title: Uninstall-NetworkControllerCluster
ms.assetid: D3AC9AAD-4EE0-4533-B187-E2BA0E4AF07A
---

# Uninstall-NetworkControllerCluster

## SYNOPSIS
Uninstalls the network controller cluster.

## SYNTAX

```
Uninstall-NetworkControllerCluster [-Force] [-ComputerName <String>] [-UseSsl] [-Credential <PSCredential>]
 [-CertificateThumbprint <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Uninstall-NetworkControllerCluster** cmdlet uninstalls the network controller cluster.
If the network controller application is deployed on top of the cluster, that is also removed.

## EXAMPLES

### Example 1: Uninstall a network controller cluster by name
```
PS C:\> Uninstall-NetworkControllerCluster -ComputerName "Node1.Contoso.com"
```

This command uninstalls the network controller cluster node named.
Node1.Contoso.com.
If *ComputerName* is not specified, this cmdlet will remove the network controller cluster on the local computer.

## PARAMETERS

### -CertificateThumbprint
Specifies the digital public key X.509 certificate of a user account that has permission to perform this action.
Specify the certificate thumbprint of the certificate.
Specify this parameter only if you run this cmdlet on a computer that is not part of the network controller cluster.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ComputerName
Specifies the name of the network controller node on which this cmdlet operates.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

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

### -Credential
Specifies a user credential that has permission to perform this action.
The default is the current user.
Specify this parameter only if you run this cmdlet on a computer that is not part of the network controller cluster.

```yaml
Type: PSCredential
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Forces the command to run without asking for user confirmation.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UseSsl
Indicates that the remote computer uses the Secure Sockets Layer (SSL) protocol to establish a connection to the Network Controller node.
The default value of this parameter is false.
Specify this parameter only if you run this cmdlet on a computer that is not part of the network controller cluster.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-NetworkControllerCluster](./Get-NetworkControllerCluster.md)

[Install-NetworkControllerCluster](./Install-NetworkControllerCluster.md)

[Repair-NetworkControllerCluster](./Repair-NetworkControllerCluster.md)

[Set-NetworkControllerCluster](./Set-NetworkControllerCluster.md)

