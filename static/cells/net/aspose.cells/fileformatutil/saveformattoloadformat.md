##FileFormatUtil.SaveFormatToLoadFormat
FileFormatUtil method. Converts a SaveFormat value to a LoadFormat value if possible
## FileFormatUtil.SaveFormatToLoadFormat method
Converts a SaveFormat value to a LoadFormat value if possible.
```csharp
public static LoadFormat SaveFormatToLoadFormat(SaveFormat saveFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The save format. |
### Return Value
The load format
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FileFormatUtilMethodSaveFormatToLoadFormatWithSaveFormatDemo
{
public static void Run()
{
// Demonstrate SaveFormatToLoadFormat conversions
Console.WriteLine("SaveFormat to LoadFormat Conversion Examples:");
LoadFormat excel97To2003 = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Excel97To2003);
Console.WriteLine($"SaveFormat.Excel97To2003 -> {excel97To2003}");
LoadFormat xlsx = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Xlsx);
Console.WriteLine($"SaveFormat.Xlsx -> {xlsx}");
LoadFormat tsv = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Tsv);
Console.WriteLine($"SaveFormat.Tsv -> {tsv}");
LoadFormat ods = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Ods);
Console.WriteLine($"SaveFormat.Ods -> {ods}");
LoadFormat xlsb = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Xlsb);
Console.WriteLine($"SaveFormat.Xlsb -> {xlsb}");
}
}
}
```
### See Also
* enum [LoadFormat](../../loadformat/)
* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
