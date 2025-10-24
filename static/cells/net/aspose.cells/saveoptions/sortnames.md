##SaveOptions.SortNames
SaveOptions property. Indicates whether sorting defined names before saving file
## SaveOptions.SortNames property
Indicates whether sorting defined names before saving file.
```csharp
public bool SortNames { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SaveOptionsPropertySortNamesDemo
{
public static void Run()
{
// Create a new Workbook object
Workbook workbook = new Workbook();
// Add sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("Item1");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("Item2");
worksheet.Cells["B3"].PutValue(200);
// Create a named range
worksheet.Cells.CreateRange("A2:B3").Name = "MyDataRange";
// Create save options with SortNames enabled
XlsSaveOptions saveOptions = new XlsSaveOptions
{
SortNames = true
};
// Save the workbook
workbook.Save("SortedNamesExample.xls", saveOptions);
Console.WriteLine("Workbook saved with sorted named ranges.");
}
}
}
```
### See Also
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
