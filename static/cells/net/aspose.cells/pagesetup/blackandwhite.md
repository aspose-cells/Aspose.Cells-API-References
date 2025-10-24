##PageSetup.BlackAndWhite
PageSetup property. Represents if elements of the document will be printed in black and white
## PageSetup.BlackAndWhite property
Represents if elements of the document will be printed in black and white.
```csharp
public bool BlackAndWhite { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyBlackAndWhiteDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the PageSetup object
PageSetup pageSetup = worksheet.PageSetup;
// Set BlackAndWhite property to true
pageSetup.BlackAndWhite = true;
Console.WriteLine("BlackAndWhite set to: " + pageSetup.BlackAndWhite);
// Change BlackAndWhite property to false
pageSetup.BlackAndWhite = false;
Console.WriteLine("BlackAndWhite changed to: " + pageSetup.BlackAndWhite);
// Save the workbook
workbook.Save("PageSetupBlackAndWhiteDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
