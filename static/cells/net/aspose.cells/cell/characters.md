##Cell.Characters
Cell method. Returns a Characters object that represents a range of characters within the cell text
## Cell.Characters method
Returns a Characters object that represents a range of characters within the cell text.
```csharp
public FontSetting Characters(int startIndex, int length)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | The index of the start of the character. |
| length | Int32 | The number of characters. |
### Return Value
Characters object.
### Remarks
This method only works on cell with string value.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class CellMethodCharactersWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].PutValue("Helloworld");
cells["A1"].Characters(5, 5).Font.IsBold = true;
cells["A1"].Characters(5, 5).Font.Color = Color.Blue;
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
