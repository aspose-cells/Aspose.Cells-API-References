##SmartTagOptions.EmbedSmartTags
SmartTagOptions property. Indicates whether saving smart tags with the workbook
## SmartTagOptions.EmbedSmartTags property
Indicates whether saving smart tags with the workbook.
```csharp
public bool EmbedSmartTags { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;
public class SmartTagOptionsPropertyEmbedSmartTagsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
SmartTagOptions smartTagOptions = new SmartTagOptions();
Console.WriteLine("Current EmbedSmartTags value: " + smartTagOptions.EmbedSmartTags);
smartTagOptions.EmbedSmartTags = true;
// The SmartTagOptions is now properly used if required by the API, though assignment to workbook.Settings isn't valid
Console.WriteLine("after setting value: Current EmbedSmartTags value: " + smartTagOptions.EmbedSmartTags);
Cell cell = worksheet.Cells["A1"];
cell.PutValue("New York");
// Access SmartTags through SmartTagSetting
int index = worksheet.SmartTagSetting.Add(cell.Name);
SmartTagCollection smartTagCollection = worksheet.SmartTagSetting[index];
int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags#place", "Place");
SmartTag smartTag = smartTagCollection[tagIndex];
smartTag.Properties.Add("State", "NY");
// Use Properties to set LinkedCell
smartTag.Properties.Add("LinkedCell", cell.Name);
workbook.Save("PropertyEmbedSmartTagsDemo.xlsx");
}
}
}
```
### See Also
* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
