##Enum VisibilityType
Aspose.Cells.VisibilityType enum. Represents the states for sheet visibility
## VisibilityType enumeration
Represents the states for sheet visibility.
```csharp
public enum VisibilityType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Visible | `0` | Indicates the sheet is visible. |
| Hidden | `1` | Indicates the sheet is hidden, but can be shown by the user via the user interface. |
| VeryHidden | `2` | Indicates the sheet is hidden and cannot be shown in the user interface (UI). This state is only available programmatically. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class VisibilityTypeDemo
{
public static void VisibilityTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
workbook.Worksheets.Add("NewSheet");
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set the name of the worksheet
worksheet.Name = "DemoSheet";
// Set the visibility of the worksheet to Hidden
worksheet.VisibilityType = VisibilityType.Hidden;
// Save the workbook
workbook.Save("VisibilityTypeExample.xlsx");
// Output to indicate the process is complete
Console.WriteLine("Workbook saved with the worksheet visibility set to Hidden.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
