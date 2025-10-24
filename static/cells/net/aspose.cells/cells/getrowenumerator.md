##Cells.GetRowEnumerator
Cells method. Gets the rows enumerator
## Cells.GetRowEnumerator method
Gets the rows enumerator.
```csharp
[Obsolete("Use RowCollection.GetEnumerator() method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetRowEnumerator()
```
### Return Value
The rows enumerator.
### Remarks
NOTE: This member is now obsolete. Instead, please use RowCollection.GetEnumerator() method. This method will be removed 12 months later since May 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Collections;
public class CellsMethodGetRowEnumeratorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Row 1 Data");
worksheet.Cells["A3"].PutValue("Row 3 Data");
worksheet.Cells["A5"].PutValue("Row 5 Data");
try
{
// Get row enumerator from Cells collection
IEnumerator enumerator = worksheet.Cells.GetRowEnumerator();
Console.WriteLine("Iterating through rows containing data:");
while (enumerator.MoveNext())
{
Row row = (Row)enumerator.Current;
Cell cell = row.GetCellOrNull(0); // Get first cell in row
string cellValue = cell != null ? cell.Value.ToString() : "empty";
Console.WriteLine($"Row {row.Index}: First cell value = {cellValue}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetRowEnumerator method: {ex.Message}");
}
// Save the workbook
workbook.Save("MethodGetRowEnumeratorDemo.xlsx");
}
}
}
```
### See Also
* method [GetEnumerator](../../rowcollection/getenumerator/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
