##OdsCellField.FieldType
OdsCellField property. Gets and sets the type of the field
## OdsCellField.FieldType property
Gets and sets the type of the field.
```csharp
public OdsCellFieldType FieldType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class OdsCellFieldPropertyFieldTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add ODS cell fields with different field types and format strings
sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "Title Format");
sheet.Cells.OdsCellFields.Add(1, 0, OdsCellFieldType.SheetName, "SheetName Format");
// Demonstrate FieldType property usage
Console.WriteLine("Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
Console.WriteLine("Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);
// Save and reload to demonstrate persistence
workbook.Save("output.ods");
workbook = new Workbook("output.ods");
sheet = workbook.Worksheets[0];
// Verify FieldType after reload
Console.WriteLine("After reload - Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
Console.WriteLine("After reload - Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);
}
}
}
```
### See Also
* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)
