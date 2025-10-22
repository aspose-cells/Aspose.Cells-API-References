##OdsCellField.CustomFormat
OdsCellField property. Represents the custom format of the fields value
## OdsCellField.CustomFormat property
Represents the custom format of the field's value.
```csharp
public string CustomFormat { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class OdsCellFieldPropertyCustomFormatDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;
// Date field with custom format
odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
// Sheet name field without custom format
odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
// Title field with custom format (demonstrating string format)
odsCellFields.Add(2, 0, OdsCellFieldType.Title, "Title Format: @");
odsCellFields.UpdateFieldsValue();
foreach (OdsCellField field in odsCellFields)
{
worksheet.Cells[field.Row, field.Column].PutValue(
$"Type: {field.FieldType}, Format: {field.CustomFormat ?? "None"}");
}
workbook.Save("OdsCellFieldCustomFormatDemo.ods");
}
}
}
```
### See Also
* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)
