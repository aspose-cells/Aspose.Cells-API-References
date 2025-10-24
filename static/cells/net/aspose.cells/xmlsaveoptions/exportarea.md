##XmlSaveOptions.ExportArea
XmlSaveOptions property. Gets or sets the exporting range
## XmlSaveOptions.ExportArea property
Gets or sets the exporting range.
```csharp
public CellArea ExportArea { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlSaveOptionsPropertyExportAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Fill data in the worksheet
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create XmlSaveOptions and set ExportArea
XmlSaveOptions saveOptions = new XmlSaveOptions
{
ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
};
// Save only the specified area to XML
workbook.Save("ExportAreaDemo.xml", saveOptions);
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
