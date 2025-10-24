##XmlSaveOptions.HasHeaderRow
XmlSaveOptions property. Indicates whether the range contains header row
## XmlSaveOptions.HasHeaderRow property
Indicates whether the range contains header row.
```csharp
public bool HasHeaderRow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlSaveOptionsPropertyHasHeaderRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add header row and data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create XML save options
XmlSaveOptions saveOptions = new XmlSaveOptions();
saveOptions.HasHeaderRow = true; // Demonstrate HasHeaderRow property
saveOptions.SheetNameAsElementName = true;
// Save as XML file
workbook.Save("output.xml", saveOptions);
Console.WriteLine("XML file saved with HasHeaderRow=true");
}
}
}
```
### See Also
* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
