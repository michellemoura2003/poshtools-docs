---
external help file: PowerShellToolsPro.Cmdlets.dll-Help.xml
online version: null
schema: 2.0.0
---

# ConvertTo-PowerShell

{% hint style="info" %}
Requires [PowerShell Pro Tools](https://ironmansoftware.com/poshtools)
{% endhint %}

## SYNOPSIS

Converts C\# code to PowerShell script.

## SYNTAX

### PathByPipeline

```text
ConvertTo-PowerShell -CSharpFile <FileInfo>
```

### Path

```text
ConvertTo-PowerShell -CSharpFilePath <String>
```

### Text

```text
ConvertTo-PowerShell -CSharpCode <String>
```

## DESCRIPTION

Converts C\# code to PowerShell script.

## EXAMPLES

### Example 1

```text
PS C:\> ConvertTo-PowerShell -CSharpCode "void CreateDate(int year) { new DateTime(year); }"
```

Converts the CreateDate method to a PowerShell function.

### Example 2

```text
PS C:\> ConvertTo-PowerShell -CSharpFilePath .\*.cs
```

Converts all the CS files into PowerShell script and returns them as a collection of strings.

### Example 3

```text
PS C:\> Get-ChildItem .\*.cs | ConvertTo-PowerShell
```

Converts all the piped CS files into PowerShell script and returns them as a collection of strings.

## PARAMETERS

### -CSharpCode

C\# code to convert

```yaml
Type: String
Parameter Sets: Text
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CSharpFilePath

C\# file \(cs\) to convert

```yaml
Type: String
Parameter Sets: Path
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: True
```

### -CSharpFile

C\# file \(cs\) to convert

```yaml
Type: FileInfo
Parameter Sets: PathByPipeline
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## INPUTS

### System.String

## OUTPUTS

### System.String

## NOTES

## RELATED LINKS

