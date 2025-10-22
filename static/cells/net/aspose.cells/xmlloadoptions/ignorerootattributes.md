##XmlLoadOptions.IgnoreRootAttributes
XmlLoadOptions property. Indicates whether ignore attributes of the root element
## XmlLoadOptions.IgnoreRootAttributes property
Indicates whether ignore attributes of the root element.
```csharp
public bool IgnoreRootAttributes { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlLoadOptionsPropertyIgnoreRootAttributesDemo
{
public static void Run()
{
// Create XML load options and set IgnoreRootAttributes
XmlLoadOptions options = new XmlLoadOptions();
options.IgnoreRootAttributes = true;
// Load XML file with the options
Workbook workbook = new Workbook("example.xml", options);
// Access data from the loaded XML
string cellValue = workbook.Worksheets[0].Cells["AH8"].StringValue;
Console.WriteLine("Cell AH8 value: " + cellValue);
// Save as XLSX
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
