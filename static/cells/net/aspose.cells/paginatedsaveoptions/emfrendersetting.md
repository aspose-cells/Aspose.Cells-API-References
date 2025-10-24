##PaginatedSaveOptions.EmfRenderSetting
PaginatedSaveOptions property. Setting for rendering Emf metafile
## PaginatedSaveOptions.EmfRenderSetting property
Setting for rendering Emf metafile.
```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```
### Remarks
EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When EmfPlusPrefer is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is EmfOnly.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyEmfRenderSettingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
// Create image for EMF demonstration
worksheet.Pictures.Add(10, 10, "example.png");
// Configure save options with EMF settings using PdfSaveOptions
PdfSaveOptions options = new PdfSaveOptions()
{
EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer
};
// Save the workbook with EMF settings
workbook.Save("EmfRenderSettingDemo.pdf", options);
}
}
}
```
### See Also
* enum [EmfRenderSetting](../../emfrendersetting/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
