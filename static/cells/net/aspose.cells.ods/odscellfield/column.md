##OdsCellField.Column
OdsCellField property. Get and sets the column index of the cell
## OdsCellField.Column property
Get and sets the column index of the cell.
```csharp
public int Column { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class OdsCellFieldPropertyColumnDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;
// Add fields with different types and demonstrate Column property
odsCellFields.Add(0, 2, OdsCellFieldType.Date, "yyyy-mm-dd");
odsCellFields.Add(1, 3, OdsCellFieldType.SheetName, null);
odsCellFields.Add(2, 4, OdsCellFieldType.Title, null);
// Access and display Column property
Console.WriteLine("Field Columns:");
foreach (OdsCellField field in odsCellFields)
{
Console.WriteLine($"Type: {field.FieldType}, Column: {field.Column}");
worksheet.Cells[field.Row, field.Column].PutValue($"Column: {field.Column}");
}
odsCellFields.UpdateFieldsValue();
workbook.Save("OdsCellFieldColumnDemo.ods");
}
}
}
```
### See Also
* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)
