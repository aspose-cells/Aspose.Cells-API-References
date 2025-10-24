##XmlLoadOptions.IsXmlMap
XmlLoadOptions property. Indicates whether mapping xml to Excel. The default value is false
## XmlLoadOptions.IsXmlMap property
Indicates whether mapping xml to Excel. The default value is false.
```csharp
public bool IsXmlMap { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlLoadOptionsPropertyIsXmlMapDemo
{
public static void Run()
{
// Create an instance of XmlLoadOptions
XmlLoadOptions options = new XmlLoadOptions();
// Enable XML mapping when loading the file
options.IsXmlMap = true;
// Load an XML file into a Workbook using the specified options
Workbook workbook = new Workbook("sample.xml", options);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Display some data from the loaded XML to demonstrate successful mapping
Console.WriteLine("Data from loaded XML:");
Console.WriteLine(worksheet.Cells["A1"].StringValue);
Console.WriteLine(worksheet.Cells["A2"].StringValue);
// Save the workbook to a new Excel file
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
