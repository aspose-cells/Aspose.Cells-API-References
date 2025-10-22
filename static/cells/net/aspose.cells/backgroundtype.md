##Enum BackgroundType
Aspose.Cells.BackgroundType enum. Enumerates cell background pattern types
## BackgroundType enumeration
Enumerates cell background pattern types.
```csharp
public enum BackgroundType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| DiagonalCrosshatch | `9` | Represents diagonal crosshatch pattern. |
| DiagonalStripe | `8` | Represents diagonal stripe pattern. |
| Gray6 | `18` | Represents 6.25% gray pattern |
| Gray12 | `17` | Represents 12.5% gray pattern |
| Gray25 | `4` | Represents 25% gray pattern. |
| Gray50 | `2` | Represents 50% gray pattern. |
| Gray75 | `3` | Represents 75% gray pattern. |
| HorizontalStripe | `5` | Represents horizontal stripe pattern. |
| None | `0` | Represents no background. |
| ReverseDiagonalStripe | `7` | Represents reverse diagonal stripe pattern. |
| Solid | `1` | Represents solid pattern. |
| ThickDiagonalCrosshatch | `10` | Represents thick diagonal crosshatch pattern. |
| ThinDiagonalCrosshatch | `16` | Represents thin diagonal crosshatch pattern. |
| ThinDiagonalStripe | `14` | Represents thin diagonal stripe pattern. |
| ThinHorizontalCrosshatch | `15` | Represents thin horizontal crosshatch pattern. |
| ThinHorizontalStripe | `11` | Represents thin horizontal stripe pattern. |
| ThinReverseDiagonalStripe | `13` | Represents thin reverse diagonal stripe pattern. |
| ThinVerticalStripe | `12` | Represents thin vertical stripe pattern. |
| VerticalStripe | `6` | Represents vertical stripe pattern. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class BackgroundTypeDemo
{
public static void BackgroundTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet in the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Access a cell from the worksheet
Cell cell = worksheet.Cells["A1"];
// Set the value of the cell
cell.PutValue("Hello, Aspose!");
// Create a style object
Style style = cell.GetStyle();
// Set the background pattern type
style.Pattern = BackgroundType.DiagonalStripe;
// Set the foreground color
style.ForegroundColor = Color.Red;
// Set the background color
style.BackgroundColor = Color.Green;
// Apply the style to the cell
cell.SetStyle(style);
// Save the workbook
workbook.Save("BackgroundTypeExample.xlsx");
workbook.Save("BackgroundTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
