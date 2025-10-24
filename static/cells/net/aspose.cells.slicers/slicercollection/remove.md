##SlicerCollection.Remove
SlicerCollection method. Remove the specified Slicer
## SlicerCollection.Remove method
Remove the specified Slicer
```csharp
public void Remove(Slicer slicer)
```
| Parameter | Type | Description |
| --- | --- | --- |
| slicer | Slicer | The Slicer object |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class SlicerCollectionMethodRemoveWithSlicerDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Column1");
worksheet.Cells["A2"].PutValue("Item1");
worksheet.Cells["A3"].PutValue("Item2");
ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "A3", true)];
SlicerCollection slicers = worksheet.Slicers;
slicers.Add(table, 0, "C1");
slicers.Add(table, 0, "C5");
Slicer delSlicer = slicers[0];
slicers.Remove(delSlicer);
}
}
}
```
### See Also
* class [Slicer](../../slicer/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
