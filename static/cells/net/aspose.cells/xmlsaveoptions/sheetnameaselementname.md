##XmlSaveOptions.SheetNameAsElementName
XmlSaveOptions property. Indicates whether exporting sheets name as the name of the element
## XmlSaveOptions.SheetNameAsElementName property
Indicates whether exporting sheet's name as the name of the element.
```csharp
public bool SheetNameAsElementName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlSaveOptionsPropertySheetNameAsElementNameDemo
{
public static void Run()
{
// Create a sample workbook with data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Name = "EmployeeData";
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John Doe");
// Save with SheetNameAsElementName = true (default)
XmlSaveOptions saveOptions = new XmlSaveOptions();
saveOptions.SheetNameAsElementName = true;
workbook.Save("output_with_sheetname.xml", saveOptions);
// Save with SheetNameAsElementName = false
saveOptions.SheetNameAsElementName = false;
workbook.Save("output_without_sheetname.xml", saveOptions);
Console.WriteLine("XML files created successfully with different SheetNameAsElementName settings.");
}
}
}
```
### See Also
* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
