##ReferredArea.StartColumn
ReferredArea property. The start column of the area
## ReferredArea.StartColumn property
The start column of the area.
```csharp
public int StartColumn { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReferredAreaPropertyStartColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Apple");
worksheet.Cells["B1"].PutValue("Banana");
worksheet.Cells["C1"].PutValue("Cherry");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["C2"].PutValue(30);
// Create a named range that refers to B1:C2
int index = workbook.Worksheets.Names.Add("MyRange");
Name name = workbook.Worksheets.Names[index];
name.RefersTo = "=Sheet1!B1:C2";
// Get the referred area with recalculate set to false
ReferredArea referredArea = name.GetReferredAreas(false)[0];
// Demonstrate StartColumn property
Console.WriteLine("Start Column: " + referredArea.StartColumn);
Console.WriteLine("End Column: " + referredArea.EndColumn);
// Print values in the referred area using StartColumn
Cells cells = worksheet.Cells;
for (int row = referredArea.StartRow; row <= referredArea.EndRow; row++)
{
for (int col = referredArea.StartColumn; col <= referredArea.EndColumn; col++)
{
Console.WriteLine(cells[row, col].Name + ": " + cells[row, col].Value);
}
}
}
}
}
```
### See Also
* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
