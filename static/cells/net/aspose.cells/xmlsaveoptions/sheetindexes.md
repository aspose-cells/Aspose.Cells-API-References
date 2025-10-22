##XmlSaveOptions.SheetIndexes
XmlSaveOptions property. Represents the indexes of exported sheets
## XmlSaveOptions.SheetIndexes property
Represents the indexes of exported sheets.
```csharp
public int[] SheetIndexes { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class XmlSaveOptionsPropertySheetIndexesDemo
{
public static void Run()
{
// Create a new workbook with multiple sheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Populate some data in all sheets
for (int i = 0; i < workbook.Worksheets.Count; i++)
{
Worksheet sheet = workbook.Worksheets[i];
sheet.Cells["A1"].PutValue("Data in " + sheet.Name);
}
// Create XmlSaveOptions instance
XmlSaveOptions options = new XmlSaveOptions();
// Initially export all sheets (SheetIndexes is null)
Console.WriteLine("Initial SheetIndexes value: " + (options.SheetIndexes == null ? "null (all sheets)" : string.Join(",", options.SheetIndexes)));
// Set to export only first and third sheets (indexes 0 and 2)
options.SheetIndexes = new int[] { 0, 2 };
// Save with selected sheets only
workbook.Save("XmlExportSelectedSheets.xml", options);
// Change to export only the second sheet (index 1)
options.SheetIndexes = new int[] { 1 };
// Save with different sheet selection
workbook.Save("XmlExportSingleSheet.xml", options);
// Set SheetIndexes to null to export all sheets
options.SheetIndexes = null;
workbook.Save("XmlExportAllSheets.xml", options);
}
}
}
```
### See Also
* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
