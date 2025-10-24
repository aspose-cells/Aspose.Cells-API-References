##OdsCellFieldCollection.Item
OdsCellFieldCollection property. Gets the field by the index
## OdsCellFieldCollection indexer (1 of 2)
Gets the field by the index.
```csharp
public OdsCellField this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class OdsCellFieldCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add ODS cell fields with format parameter
sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "");
sheet.Cells.OdsCellFields.Add(0, 1, OdsCellFieldType.SheetName, "");
// Access fields using Item property
OdsCellField titleField = sheet.Cells.OdsCellFields[0];
OdsCellField sheetNameField = sheet.Cells.OdsCellFields[1];
// Output field types
Console.WriteLine("Field 0 Type: " + titleField.FieldType);
Console.WriteLine("Field 1 Type: " + sheetNameField.FieldType);
// Save and reload
workbook.Save("output.ods");
workbook = new Workbook("output.ods");
sheet = workbook.Worksheets[0];
// Verify persisted fields
Console.WriteLine("Reloaded Field 0 Type: " + sheet.Cells.OdsCellFields[0].FieldType);
Console.WriteLine("Reloaded Field 1 Type: " + sheet.Cells.OdsCellFields[1].FieldType);
}
}
}
```
### See Also
* class [OdsCellField](../../odscellfield/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)
## OdsCellFieldCollection indexer (2 of 2)
Gets the field by row and column index.
```csharp
public OdsCellField this[int row, int column] { get; }
```
| Parameter | Description |
| --- | --- |
| row | The row index. |
| column | The column index. |
### See Also
* class [OdsCellField](../../odscellfield/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)
