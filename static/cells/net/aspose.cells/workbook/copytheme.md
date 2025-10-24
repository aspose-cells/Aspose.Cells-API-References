##Workbook.CopyTheme
Workbook method. Copies the theme from another workbook
## Workbook.CopyTheme method
Copies the theme from another workbook.
```csharp
public void CopyTheme(Workbook source)
```
| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source workbook. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCopyThemeWithWorkbookDemo
{
public static void Run()
{
// Create source workbook (theme is automatically set when opening a template file)
Workbook sourceWorkbook = new Workbook(FileFormatType.Xlsx);
// Create destination workbook
Workbook destWorkbook = new Workbook();
// Copy theme from source to destination workbook
destWorkbook.CopyTheme(sourceWorkbook);
// Save the destination workbook
destWorkbook.Save("output_with_theme.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
