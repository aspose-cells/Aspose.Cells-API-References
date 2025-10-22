##RowCollection.GetEnumerator
RowCollection method. Gets an enumerator that iterates rows through this collection
## GetEnumerator() {#getenumerator}
Gets an enumerator that iterates rows through this collection
```csharp
public IEnumerator GetEnumerator()
```
### Return Value
The row enumerator which will traverse all existing rows in this collection.
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowCollectionMethodGetEnumeratorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set row heights for demonstration
worksheet.Cells.SetRowHeight(0, 15);
worksheet.Cells.SetRowHeight(1, 20);
worksheet.Cells.SetRowHeight(2, 25);
IEnumerator enumerator = worksheet.Cells.Rows.GetEnumerator();
while (enumerator.MoveNext())
{
Row row = (Row)enumerator.Current;
Console.WriteLine($"Row index: {row.Index}, Height: {row.Height}");
}
}
}
}
```
### See Also
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetEnumerator(bool, bool) {#getenumerator_1}
Gets an enumerator that iterates rows through this collection
```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```
| Parameter | Type | Description |
| --- | --- | --- |
| reversed | Boolean | whether enumerate rows in reversed order |
| sync | Boolean | whether the returned enumerator should check the modification of row collection and keep synchronized with it. |
### Return Value
The row enumerator which will traverse all existing rows in this collection.
### Remarks
If the row collection will be modified(by operations that may cause new Row be instantiated or existing Row be removed) during the traversal with the enumerator, synchronized enumerator should be used instead of normal enumerator so that the traversal can continue from the position just after the one has been traversed by the last MoveNext(). However, together with the advantage that no element be skipped or traversed repeatedly, the disadvantage for synchronized enumerator is that the performance will be degraded a bit when comparing with normal enumerator.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Collections;
public class RowCollectionMethodGetEnumeratorWithBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to rows
for (int i = 0; i < 5; i++)
{
Row row = worksheet.Cells.Rows[i];
row[0].PutValue($"Row {i + 1}");
}
try
{
// Get the RowCollection
RowCollection rows = worksheet.Cells.Rows;
// Call GetEnumerator with parameters (reversed: true, sync: false)
IEnumerator enumerator = rows.GetEnumerator(true, false);
Console.WriteLine("Iterating rows in reverse order:");
while (enumerator.MoveNext())
{
Row row = (Row)enumerator.Current;
Console.WriteLine(row[0].StringValue);
}
// Call GetEnumerator with parameters (reversed: false, sync: true)
enumerator = rows.GetEnumerator(false, true);
Console.WriteLine("\nIterating rows in normal order (synchronized):");
while (enumerator.MoveNext())
{
Row row = (Row)enumerator.Current;
Console.WriteLine(row[0].StringValue);
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
}
// Save the result
workbook.Save("RowCollectionGetEnumeratorDemo.xlsx");
}
}
}
```
### See Also
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
