##LineFormat.Equals
LineFormat method. Determines whether this instance has the same value as another specified LineFormat object
## LineFormat.Equals method
Determines whether this instance has the same value as another specified [`LineFormat`](../) object.
```csharp
public override bool Equals(object obj)
```
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The [`LineFormat`](../) object to compare with this instance. |
### Return Value
true if the value of the obj parameter is the same as the value of this instance; otherwise, false. If obj is null, this method returns false.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LineFormatMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape to the worksheet
worksheet.Shapes.AddLine(1, 1, 10, 10, 100, 0);
// Get the line format of the first shape
LineFormat lineFmt1 = worksheet.Shapes[0].Line;
LineFormat lineFmt2 = worksheet.Shapes[0].Line;
// Compare the line formats using Equals method
if (lineFmt1.Equals((object)lineFmt2))
{
Console.WriteLine("The line formats are equal.");
}
else
{
Console.WriteLine("The line formats are not equal.");
}
}
}
}
```
### See Also
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
