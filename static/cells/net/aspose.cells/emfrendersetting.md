##Enum EmfRenderSetting
Aspose.Cells.EmfRenderSetting enum. Setting for rendering Emf metafile
## EmfRenderSetting enumeration
Setting for rendering Emf metafile.
```csharp
public enum EmfRenderSetting
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| EmfOnly | `0` | Only rendering Emf records. |
| EmfPlusPrefer | `1` | Prefer rendering EmfPlus records. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class CellsClassEmfRenderSettingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
worksheet.Cells["A2"].PutValue("Using EmfOnly setting");
// Create image options with EMF render setting
ImageOrPrintOptions options = new ImageOrPrintOptions
{
EmfRenderSetting = EmfRenderSetting.EmfOnly
};
// Create a sheet render with the options
SheetRender render = new SheetRender(worksheet, options);
// Save the first page as EMF image
render.ToImage(0, "EmfRenderSettingDemo.emf");
Console.WriteLine("EMF file created successfully with EmfOnly setting.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
