##FileFormatUtil.IsTemplateFormat
FileFormatUtil method. Returns true if the extension is .xlt .xltX .xltm.ots
## FileFormatUtil.IsTemplateFormat method
Returns true if the extension is .xlt, .xltX, .xltm,.ots.
```csharp
public static bool IsTemplateFormat(string extension)
```
| Parameter | Type | Description |
| --- | --- | --- |
| extension | String |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FileFormatUtilMethodIsTemplateFormatWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
string extension = ".xltx";
try
{
bool isTemplate = FileFormatUtil.IsTemplateFormat(extension);
Console.WriteLine($"Is '{extension}' a template format? {isTemplate}");
if (isTemplate)
{
SaveFormat saveFormat = FileFormatUtil.ExtensionToSaveFormat(extension);
workbook.Save($"IsTemplateFormatDemo{extension}", saveFormat);
Console.WriteLine($"Workbook saved as template format: {extension}");
}
}
catch (ArgumentException argEx)
{
Console.WriteLine($"Invalid argument: {argEx.Message}");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
