##CellRichValue.AltText
CellRichValue property. Gets the alt text associated with the image
## CellRichValue.AltText property
Gets the alt text associated with the image.
```csharp
public virtual string AltText { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellRichValuePropertyAltTextDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["C4"];
cell.GetRichValue().AltText = "test alt text";
Console.WriteLine("AltText: " + cell.GetRichValue().AltText);
}
}
}
```
### See Also
* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
