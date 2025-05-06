---
title: SpreadsheetLocker.Process
second_title: Aspose.Cells for .NET API Reference
description: SpreadsheetLocker method. Locks spreadsheet file with specified settings
type: docs
url: /net/aspose.cells.lowcode/spreadsheetlocker/process/
---
## Process(string, string, string, string) {#process_3}

Locks spreadsheet file with specified settings.

```csharp
public static void Process(string templateFile, string resultFile, string openPassword, 
    string writePassword)
```

| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | String | The template file to be locked |
| resultFile | String | The resultant file |
| openPassword | String | Password for file encryption |
| writePassword | String | Password for protection of modifying spreadsheet |

### See Also

* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string) {#process_1}

Locks spreadsheet file with specified settings.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for output and saving |
| openPassword | String | Password for file encryption |
| writePassword | String | Password for protection of modifying spreadsheet |

### Examples

```csharp
// Called: SpreadsheetLocker.Process(new LowCodeLoadOptions() { InputStream = stream },
private void Method_String_(Stream stream, string fnTail)
        {
            SpreadsheetLocker.Process(new LowCodeLoadOptions() { InputStream = stream },
                new LowCodeSaveOptions()
                {
                    OutputFile = Constants.checkPath + &quot;License/LowCodeLock&quot; + fnTail,
                }, &quot;123456&quot;, &quot;234567&quot;);
        }
```

### See Also

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) {#process_2}

Locks spreadsheet file with specified settings.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword, string workbookPassword, ProtectionType workbookType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for output and saving |
| openPassword | String | Password for file encryption |
| writePassword | String | Password for protection of modifying spreadsheet |
| workbookPassword | String | Password for protection of the workbook |
| workbookType | ProtectionType | Protection type to protect the workbook |

### See Also

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) {#process}

Locks spreadsheet file with specified settings.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeProtectionProvider provider)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for output and saving |
| provider | AbstractLowCodeProtectionProvider | Implementation to provide protections settings |

### See Also

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeProtectionProvider](../../abstractlowcodeprotectionprovider/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


