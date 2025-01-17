---
external help file:
Module Name: Microsoft.Graph.CloudCommunications
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.cloudcommunications/invoke-mgplaycommunicationcallprompt
schema: 2.0.0
---

# Invoke-MgPlayCommunicationCallPrompt

## SYNOPSIS
Invoke action playPrompt

## SYNTAX

### PlayExpanded (Default)
```
Invoke-MgPlayCommunicationCallPrompt -CallId <String> [-AdditionalProperties <Hashtable>]
 [-ClientContext <String>] [-Prompts <IMicrosoftGraphPrompt[]>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### Play
```
Invoke-MgPlayCommunicationCallPrompt -CallId <String>
 -BodyParameter <IPaths1Gzqcv2CommunicationsCallsCallIdMicrosoftGraphPlaypromptPostRequestbodyContentApplicationJsonSchema1>
 [-Confirm] [-WhatIf] [<CommonParameters>]
```

### PlayViaIdentity
```
Invoke-MgPlayCommunicationCallPrompt -InputObject <ICloudCommunicationsIdentity>
 -BodyParameter <IPaths1Gzqcv2CommunicationsCallsCallIdMicrosoftGraphPlaypromptPostRequestbodyContentApplicationJsonSchema1>
 [-Confirm] [-WhatIf] [<CommonParameters>]
```

### PlayViaIdentityExpanded
```
Invoke-MgPlayCommunicationCallPrompt -InputObject <ICloudCommunicationsIdentity>
 [-AdditionalProperties <Hashtable>] [-ClientContext <String>] [-Prompts <IMicrosoftGraphPrompt[]>] [-Confirm]
 [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
Invoke action playPrompt

## EXAMPLES

### Example 1: Using the Invoke-MgPlayCommunicationCallPrompt Cmdlet
```powershell
Import-Module Microsoft.Graph.CloudCommunications
$params = @{
	ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c"
	Prompts = @(
		@{
			"@odata.type" = "#microsoft.graph.mediaPrompt"
			MediaInfo = @{
				"@odata.type" = "#microsoft.graph.mediaInfo"
				Uri = "https://cdn.contoso.com/beep.wav"
				ResourceId = "1D6DE2D4-CD51-4309-8DAA-70768651088E"
			}
		}
	)
}
Invoke-MgPlayCommunicationCallPrompt -CallId $callId -BodyParameter $params
```

This example shows how to use the Invoke-MgPlayCommunicationCallPrompt Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: System.Collections.Hashtable
Parameter Sets: PlayExpanded, PlayViaIdentityExpanded
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
Type: Microsoft.Graph.PowerShell.Models.IPaths1Gzqcv2CommunicationsCallsCallIdMicrosoftGraphPlaypromptPostRequestbodyContentApplicationJsonSchema1
Parameter Sets: Play, PlayViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CallId
The unique identifier of call

```yaml
Type: System.String
Parameter Sets: Play, PlayExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClientContext
.

```yaml
Type: System.String
Parameter Sets: PlayExpanded, PlayViaIdentityExpanded
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
Type: Microsoft.Graph.PowerShell.Models.ICloudCommunicationsIdentity
Parameter Sets: PlayViaIdentity, PlayViaIdentityExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Prompts
.

```yaml
Type: Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPrompt[]
Parameter Sets: PlayExpanded, PlayViaIdentityExpanded
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

### Microsoft.Graph.PowerShell.Models.ICloudCommunicationsIdentity

### Microsoft.Graph.PowerShell.Models.IPaths1Gzqcv2CommunicationsCallsCallIdMicrosoftGraphPlaypromptPostRequestbodyContentApplicationJsonSchema1

## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPlayPromptOperation

## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER <IPaths1Gzqcv2CommunicationsCallsCallIdMicrosoftGraphPlaypromptPostRequestbodyContentApplicationJsonSchema1>: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ClientContext <String>]`: 
  - `[Prompts <IMicrosoftGraphPrompt[]>]`: 

INPUTOBJECT <ICloudCommunicationsIdentity>: Identity Parameter
  - `[AttendanceRecordId <String>]`: The unique identifier of attendanceRecord
  - `[AudioRoutingGroupId <String>]`: The unique identifier of audioRoutingGroup
  - `[CallId <String>]`: The unique identifier of call
  - `[CallRecordId <String>]`: The unique identifier of callRecord
  - `[CallTranscriptId <String>]`: The unique identifier of callTranscript
  - `[CommsOperationId <String>]`: The unique identifier of commsOperation
  - `[ContentSharingSessionId <String>]`: The unique identifier of contentSharingSession
  - `[FromDateTime <DateTime?>]`: Usage: fromDateTime={fromDateTime}
  - `[MeetingAttendanceReportId <String>]`: The unique identifier of meetingAttendanceReport
  - `[MeetingRegistrationQuestionId <String>]`: The unique identifier of meetingRegistrationQuestion
  - `[OnlineMeetingId <String>]`: The unique identifier of onlineMeeting
  - `[ParticipantId <String>]`: The unique identifier of participant
  - `[PresenceId <String>]`: The unique identifier of presence
  - `[SessionId <String>]`: The unique identifier of session
  - `[ToDateTime <DateTime?>]`: Usage: toDateTime={toDateTime}
  - `[UserId <String>]`: The unique identifier of user

## RELATED LINKS

