##OdsCellField.Row
OdsCellField property. Get and sets the row index of the cell
## OdsCellField.Row property
Get and sets the row index of the cell.
```csharp
public int Row { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class OdsCellFieldPropertyRowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;
// Add fields with different types
odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
odsCellFields.Add(2, 0, OdsCellFieldType.Title, null);
odsCellFields.UpdateFieldsValue();
// Demonstrate Row property usage
for (int i = 0; i < odsCellFields.Count; i++)
{
OdsCellField field = odsCellFields[i];
int row = field.Row; // Using Row property
worksheet.Cells[row, 1].PutValue($"Row: {row}, Type: {field.FieldType}");
}
workbook.Save("OdsCellFieldRowDemo.ods");
}
}
}
```
### See Also
* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)
