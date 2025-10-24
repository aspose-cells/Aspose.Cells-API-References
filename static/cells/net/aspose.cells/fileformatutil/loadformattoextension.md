##FileFormatUtil.LoadFormatToExtension
FileFormatUtil method. Converts a load format enumerated value into a file extension
## FileFormatUtil.LoadFormatToExtension method
Converts a load format enumerated value into a file extension.
```csharp
public static string LoadFormatToExtension(LoadFormat loadFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loaded file format. |
### Return Value
The returned extension is a lower-case string with a leading dot.
### Remarks
If it can not be converted, returns null.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FileFormatUtilMethodLoadFormatToExtensionWithLoadFormatDemo
{
public static void Run()
{
// Demonstrate LoadFormatToExtension with various LoadFormat values
Console.WriteLine("Auto format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Auto));
Console.WriteLine("CSV format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Csv));
Console.WriteLine("Excel97-2003 format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Excel97To2003));
Console.WriteLine("XLSX format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsx));
Console.WriteLine("TSV format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Tsv));
Console.WriteLine("ODS format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Ods));
Console.WriteLine("XLSB format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsb));
}
}
}
```
### See Also
* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
