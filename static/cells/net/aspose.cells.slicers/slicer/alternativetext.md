##Slicer.AlternativeText
Slicer property. Returns or sets the descriptive alternative text string of the Slicer object
## Slicer.AlternativeText property
Returns or sets the descriptive (alternative) text string of the Slicer object.
```csharp
public string AlternativeText { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class SlicerPropertyAlternativeTextDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1:A3", "", true)];
table.DisplayName = "Table1";
int slicerIndex = worksheet.Slicers.Add(table, 0, "C1");
Slicer slicer = worksheet.Slicers[slicerIndex];
slicer.AlternativeText = "AlternativeText test";
workbook.Save("SlicerAlternativeTextDemo_out.xlsx");
}
}
}
```
### See Also
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
