##XmlLoadOptions.XmlLoadOptions
XmlLoadOptions constructor. Represents the options of loading xml file
## XmlLoadOptions() {#constructor}
Represents the options of loading xml file.
```csharp
public XmlLoadOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlLoadOptionsMethodCtorDemo
{
public static void Run()
{
// Create new XML load options
XmlLoadOptions options = new XmlLoadOptions();
// Set to convert numeric or date values
options.ConvertNumericOrDate = true;
// Load workbook with options
Workbook workbook = new Workbook("input.xml", options);
// Access cell data
Cell cell = workbook.Worksheets[0].Cells["A1"];
Console.WriteLine("Cell Value: " + cell.Value);
Console.WriteLine("Cell Type: " + cell.Type);
// Save workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## XmlLoadOptions(LoadFormat) {#constructor_1}
Represents the options of loading xml file.
```csharp
public XmlLoadOptions(LoadFormat type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | LoadFormat | The load format type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class XmlLoadOptionsMethodCtorWithLoadFormatDemo
{
public static void Run()
{
try
{
// Create XmlLoadOptions instance with LoadFormat parameter
LoadFormat loadFormat = LoadFormat.Xml;
XmlLoadOptions xmlLoadOptions = new XmlLoadOptions(loadFormat);
// Set some properties of the XmlLoadOptions
xmlLoadOptions.StartCell = "A1";
xmlLoadOptions.IsXmlMap = true;
xmlLoadOptions.ConvertNumericOrDate = true;
// Create a workbook using the load options
Workbook workbook = new Workbook("sample.xml", xmlLoadOptions);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Display some information
Console.WriteLine("XML file loaded successfully with LoadFormat.Xml");
Console.WriteLine($"First cell value: {worksheet.Cells["A1"].Value}");
// Save the workbook
workbook.Save("XmlLoadOptionsCtorDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing XmlLoadOptions constructor: {ex.Message}");
}
}
}
}
```
### See Also
* enum [LoadFormat](../../loadformat/)
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
