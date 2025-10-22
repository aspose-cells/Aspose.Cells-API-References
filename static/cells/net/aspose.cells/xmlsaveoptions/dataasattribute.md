##XmlSaveOptions.DataAsAttribute
XmlSaveOptions property. Indicates whether exporting data as attributes of element
## XmlSaveOptions.DataAsAttribute property
Indicates whether exporting data as attributes of element.
```csharp
public bool DataAsAttribute { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlSaveOptionsPropertyDataAsAttributeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
// Create XML save options with DataAsAttribute set to true
XmlSaveOptions saveOptions = new XmlSaveOptions
{
DataAsAttribute = true,
SheetNameAsElementName = true
};
// Save with data as attributes
workbook.Save("DataAsAttribute_True.xml", saveOptions);
// Change to save data as elements
saveOptions.DataAsAttribute = false;
workbook.Save("DataAsAttribute_False.xml", saveOptions);
}
}
}
```
### See Also
* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
