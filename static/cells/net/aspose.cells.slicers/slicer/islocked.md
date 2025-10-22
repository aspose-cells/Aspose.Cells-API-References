##Slicer.IsLocked
Slicer property. Indicates whether the slicer shape is locked
## Slicer.IsLocked property
Indicates whether the slicer shape is locked.
```csharp
public bool IsLocked { get; set; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class SlicerPropertyIsLockedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "A3", true)];
int slicerIndex = worksheet.Slicers.Add(table, 0, "D1");
Slicer slicer = worksheet.Slicers[slicerIndex];
slicer.IsLocked = false;
worksheet.Protect(ProtectionType.All, "password", null);
workbook.Save("SlicerIsLockedDemo.xlsx");
}
}
}
```
### See Also
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
