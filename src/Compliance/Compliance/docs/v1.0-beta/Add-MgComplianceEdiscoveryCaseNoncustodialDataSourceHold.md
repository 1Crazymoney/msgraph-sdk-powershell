---
external help file:
Module Name: Microsoft.Graph.Compliance
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.compliance/add-mgcomplianceediscoverycasenoncustodialdatasourcehold
schema: 2.0.0
---

# Add-MgComplianceEdiscoveryCaseNoncustodialDataSourceHold

## SYNOPSIS
Invoke action applyHold

## SYNTAX

### ApplyExpanded (Default)
```
Add-MgComplianceEdiscoveryCaseNoncustodialDataSourceHold -CaseId <String> [-AdditionalProperties <Hashtable>]
 [-Ids <String[]>] [-PassThru] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### Apply
```
Add-MgComplianceEdiscoveryCaseNoncustodialDataSourceHold -CaseId <String> -NoncustodialDataSourceId <String>
 [-PassThru] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### Apply1
```
Add-MgComplianceEdiscoveryCaseNoncustodialDataSourceHold -CaseId <String>
 -BodyParameter <IPaths18Kl3FpComplianceEdiscoveryCasesCaseIdNoncustodialdatasourcesMicrosoftGraphEdiscoveryApplyholdPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### ApplyViaIdentity
```
Add-MgComplianceEdiscoveryCaseNoncustodialDataSourceHold -InputObject <IComplianceIdentity> [-PassThru]
 [-Confirm] [-WhatIf] [<CommonParameters>]
```

### ApplyViaIdentity1
```
Add-MgComplianceEdiscoveryCaseNoncustodialDataSourceHold -InputObject <IComplianceIdentity>
 -BodyParameter <IPaths18Kl3FpComplianceEdiscoveryCasesCaseIdNoncustodialdatasourcesMicrosoftGraphEdiscoveryApplyholdPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### ApplyViaIdentityExpanded
```
Add-MgComplianceEdiscoveryCaseNoncustodialDataSourceHold -InputObject <IComplianceIdentity>
 [-AdditionalProperties <Hashtable>] [-Ids <String[]>] [-PassThru] [-Confirm] [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
Invoke action applyHold

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: System.Collections.Hashtable
Parameter Sets: ApplyExpanded, ApplyViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
.
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: Microsoft.Graph.PowerShell.Models.IPaths18Kl3FpComplianceEdiscoveryCasesCaseIdNoncustodialdatasourcesMicrosoftGraphEdiscoveryApplyholdPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Apply1, ApplyViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CaseId
The unique identifier of case

```yaml
Type: System.String
Parameter Sets: Apply, Apply1, ApplyExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Ids
.

```yaml
Type: System.String[]
Parameter Sets: ApplyExpanded, ApplyViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, please use Get-Help -Online and see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: Microsoft.Graph.PowerShell.Models.IComplianceIdentity
Parameter Sets: ApplyViaIdentity, ApplyViaIdentity1, ApplyViaIdentityExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NoncustodialDataSourceId
The unique identifier of noncustodialDataSource

```yaml
Type: System.String
Parameter Sets: Apply
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

```yaml
Type: System.Management.Automation.SwitchParameter
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IComplianceIdentity

### Microsoft.Graph.PowerShell.Models.IPaths18Kl3FpComplianceEdiscoveryCasesCaseIdNoncustodialdatasourcesMicrosoftGraphEdiscoveryApplyholdPostRequestbodyContentApplicationJsonSchema

## OUTPUTS

### System.Boolean

## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER <IPaths18Kl3FpComplianceEdiscoveryCasesCaseIdNoncustodialdatasourcesMicrosoftGraphEdiscoveryApplyholdPostRequestbodyContentApplicationJsonSchema>: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Ids <String[]>]`: 

INPUTOBJECT <IComplianceIdentity>: Identity Parameter
  - `[CaseId <String>]`: The unique identifier of case
  - `[CaseOperationId <String>]`: The unique identifier of caseOperation
  - `[CustodianId <String>]`: The unique identifier of custodian
  - `[DataSourceId <String>]`: The unique identifier of dataSource
  - `[LegalHoldId <String>]`: The unique identifier of legalHold
  - `[NoncustodialDataSourceId <String>]`: The unique identifier of noncustodialDataSource
  - `[ReviewSetId <String>]`: The unique identifier of reviewSet
  - `[ReviewSetQueryId <String>]`: The unique identifier of reviewSetQuery
  - `[SiteSourceId <String>]`: The unique identifier of siteSource
  - `[SourceCollectionId <String>]`: The unique identifier of sourceCollection
  - `[TagId <String>]`: The unique identifier of tag
  - `[TagId1 <String>]`: The unique identifier of tag
  - `[UnifiedGroupSourceId <String>]`: The unique identifier of unifiedGroupSource
  - `[UserSourceId <String>]`: The unique identifier of userSource

## RELATED LINKS

