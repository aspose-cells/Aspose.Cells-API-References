##Class XmlDataBinding
Aspose.Cells.XmlDataBinding class. Represents Xml Data Binding information
## XmlDataBinding class
Represents Xml Data Binding information.
```csharp
public class XmlDataBinding
```
## Properties
| Name | Description |
| --- | --- |
| [Url](../../aspose.cells/xmldatabinding/url/) { get; } | Gets source url of this data binding. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class CellsClassXmlDataBindingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a list object that will use XML data binding
ListObject listObject = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 5, 4, true)];
// Get the XML data binding information (this would typically be set when importing XML data)
XmlDataBinding xmlDataBinding = listObject.XmlMap.DataBinding;
// Display the URL of the XML data source (read-only property)
Console.WriteLine("XML Data Binding Source URL: " + xmlDataBinding.Url);
// Note: In a real scenario, the Url would be set when importing XML data
// For demonstration purposes, we're showing how to access the property
// Save the workbook
workbook.Save("XmlDataBindingDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
