##CellArea.CompareTo
CellArea method. Compare two CellArea objects according to their topleft corner
## CellArea.CompareTo method
Compare two CellArea objects according to their top-left corner.
```csharp
public int CompareTo(object obj)
```
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |
### Return Value
If two corners are in different rows, then compare their row index. Otherwise compare their column index. If two corners are same, then 0 will be returned.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellAreaMethodCompareToWithObjectDemo
{
public static void Run()
{
// Create two CellArea objects for comparison
CellArea ca1 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
object ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
// Demonstrate the CompareTo method with Object parameter
int comparisonResult = ca1.CompareTo(ca2);
Console.WriteLine($"Comparison result: {comparisonResult}");
// Create another comparison with equal areas
object ca3 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
comparisonResult = ca1.CompareTo(ca3);
Console.WriteLine($"Comparison result with equal areas: {comparisonResult}");
}
}
}
```
### See Also
* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
