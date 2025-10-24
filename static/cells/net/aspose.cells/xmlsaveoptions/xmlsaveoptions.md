##XmlSaveOptions.XmlSaveOptions
XmlSaveOptions constructor. Creates options for saving xml file
## XmlSaveOptions constructor
Creates options for saving xml file.
```csharp
public XmlSaveOptions()
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue(63);
// First demo: Save as XML with SheetNameAsElementName
XmlSaveOptions saveOptions1 = new XmlSaveOptions();
saveOptions1.SheetNameAsElementName = true;
workbook.Save("output1.xml", saveOptions1);
// Second demo: Save as XML with SheetNameAsElementName and DataAsAttribute
XmlSaveOptions saveOptions2 = new XmlSaveOptions();
saveOptions2.SheetNameAsElementName = true;
saveOptions2.DataAsAttribute = true;
workbook.Save("output2.xml", saveOptions2);
Console.WriteLine("XML files created successfully.");
}
}
}
```
### See Also
* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
