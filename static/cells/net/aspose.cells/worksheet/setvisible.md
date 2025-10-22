##Worksheet.SetVisible
Worksheet method. Sets the visible options
## Worksheet.SetVisible method
Sets the visible options.
```csharp
public void SetVisible(bool isVisible, bool ignoreError)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isVisible | Boolean | Whether the worksheet is visible |
| ignoreError | Boolean | Whether to ignore error if this option is not valid. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodSetVisibleWithBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some worksheets
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Set visibility of worksheets
// First parameter: isVisible - false to hide the sheet
// Second parameter: ignoreError - true to ignore error if the sheet can't be hidden
workbook.Worksheets["Sheet2"].SetVisible(false, true);
workbook.Worksheets["Sheet3"].SetVisible(false, true);
// Save the workbook
workbook.Save("WorksheetVisibilityDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
