##Workbook.Theme
Workbook property. Gets the theme name
## Workbook.Theme property
Gets the theme name.
```csharp
public string Theme { get; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyThemeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Demonstrate getting the default theme
Console.WriteLine("Default theme: " + workbook.Theme);
// Change theme color and verify
workbook.SetThemeColor(ThemeColorType.Accent1, Color.Blue);
Color accent1 = workbook.GetThemeColor(ThemeColorType.Accent1);
Console.WriteLine("Modified Accent1 color: " + accent1);
// Save the workbook to demonstrate theme persistence
workbook.Save("ThemeDemo.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
