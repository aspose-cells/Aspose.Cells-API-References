##XmlDataBinding.Url
XmlDataBinding property. Gets source url of this data binding
## XmlDataBinding.Url property
Gets source url of this data binding.
```csharp
public string Url { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class XmlDataBindingPropertyUrlDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add two worksheets
workbook.Worksheets.Add("Sheet1");
workbook.Worksheets.Add("Sheet2");
// Add list objects and XML maps
ListObject list1 = workbook.Worksheets[0].ListObjects[0];
ListObject list2 = workbook.Worksheets[1].ListObjects[0];
// Get XML data binding URLs (Url is read-only)
string url1 = list1.XmlMap.DataBinding.Url;
string url2 = list2.XmlMap.DataBinding.Url;
// Display the URLs
Console.WriteLine("Sheet1 ListObject XML URL: " + url1);
Console.WriteLine("Sheet2 ListObject XML URL: " + url2);
// Save the workbook
workbook.Save("XmlDataBindingDemo.xlsx");
}
}
}
```
### See Also
* class [XmlDataBinding](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
