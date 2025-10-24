##OdsCellFieldCollection.Add
OdsCellFieldCollection method. Adds a field
## OdsCellFieldCollection.Add method
Adds a field.
```csharp
public int Add(int row, int column, OdsCellFieldType fieldType, string format)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
| fieldType | OdsCellFieldType | The type of the field. |
| format | String | The number format of the field. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class OdsCellFieldCollectionMethodAddWithInt32Int32OdsCellFieldTypStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;
// Add different types of fields
odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-MM-dd");
odsCellFields.Add(1, 1, OdsCellFieldType.SheetName, null);
odsCellFields.Add(2, 2, OdsCellFieldType.Title, "SampleTitle");
odsCellFields.UpdateFieldsValue();
workbook.Save("OdsCellFieldsDemo.ods");
}
}
}
```
### See Also
* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)
