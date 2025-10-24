##Hyperlink.Address
Hyperlink property. Represents the address of a hyperlink
## Hyperlink.Address property
Represents the address of a hyperlink.
```csharp
public string Address { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HyperlinkPropertyAddressDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add hyperlinks with different addresses
worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.baidu.com/");
worksheet.Hyperlinks.Add("B1", 1, 1, "http://www.google.com/");
worksheet.Hyperlinks.Add("C1", 1, 1, "Sheet1!F3");
// Access and display hyperlink addresses
HyperlinkCollection links = worksheet.Hyperlinks;
Console.WriteLine("Hyperlink Count: " + links.Count);
Console.WriteLine("Link 1 Address: " + links[0].Address);
Console.WriteLine("Link 2 Address: " + links[1].Address);
Console.WriteLine("Link 3 Address: " + links[2].Address);
// Save the workbook
workbook.Save("HyperlinkDemo.xlsx");
}
}
}
```
### See Also
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
