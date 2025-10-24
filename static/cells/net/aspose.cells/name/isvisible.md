##Name.IsVisible
Name property. Indicates whether the name is visible
## Name.IsVisible property
Indicates whether the name is visible.
```csharp
public bool IsVisible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NamePropertyIsVisibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a visible named range
int visibleIndex = workbook.Worksheets.Names.Add("VisibleRange");
Name visibleName = workbook.Worksheets.Names[visibleIndex];
visibleName.RefersTo = "=Sheet1!$A$1:$B$2";
visibleName.IsVisible = true;
// Create a hidden named range
int hiddenIndex = workbook.Worksheets.Names.Add("HiddenRange");
Name hiddenName = workbook.Worksheets.Names[hiddenIndex];
hiddenName.RefersTo = "=Sheet1!$C$1:$D$2";
hiddenName.IsVisible = false;
// Demonstrate IsVisible property
Console.WriteLine("VisibleRange IsVisible: " + visibleName.IsVisible);
Console.WriteLine("HiddenRange IsVisible: " + hiddenName.IsVisible);
// Save the workbook
workbook.Save("NameVisibilityDemo.xlsx");
}
}
}
```
### See Also
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
