##Enum SensitivityLabelMarkType
Aspose.Cells.Metas.SensitivityLabelMarkType enum. Represents the types of content marking that ought to be applied to a file
## SensitivityLabelMarkType enumeration
Represents the types of content marking that ought to be applied to a file.
```csharp
[Flags]
public enum SensitivityLabelMarkType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | None |
| Header | `1` | Header |
| Footer | `2` | Footer |
| Watermark | `4` | Watermark |
| Encryption | `8` | Encryption |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metas;
using System;
public class MetasClassSensitivityLabelMarkTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Demonstrate SensitivityLabelMarkType enum values
SensitivityLabelMarkType markType = SensitivityLabelMarkType.Watermark;
// Apply different sensitivity label marks based on the type
switch (markType)
{
case SensitivityLabelMarkType.None:
Console.WriteLine("No sensitivity label applied");
break;
case SensitivityLabelMarkType.Header:
worksheet.PageSetup.SetHeader(0, "CONFIDENTIAL");
break;
case SensitivityLabelMarkType.Footer:
worksheet.PageSetup.SetFooter(0, "INTERNAL USE ONLY");
break;
case SensitivityLabelMarkType.Watermark:
worksheet.PageSetup.SetHeader(0, "&KFF0000&DRAFT");
break;
case SensitivityLabelMarkType.Encryption:
workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
break;
}
// Save the workbook with applied sensitivity label
workbook.Save("SensitivityLabelMarkTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)
