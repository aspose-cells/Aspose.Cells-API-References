##SmartTag.Deleted
SmartTag property. Indicates whether the smart tag is deleted
## SmartTag.Deleted property
Indicates whether the smart tag is deleted.
```csharp
public bool Deleted { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;
public class SmartTagPropertyDeletedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Aspose");
sheet.Cells["A2"].PutValue("Cells");
SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
int smartTagIndex = smartTagSetting.Add(0, 0);
SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
smartTags.Add("http://docs.aspose.com", "docs");
SmartTag smartTag = smartTags[0];
smartTag.SetLink("http://www.aspose.com", "AsposeLink");
SmartTagPropertyCollection properties = smartTag.Properties;
properties.Add("Author", "Aspose");
properties.Add("Description", "Aspose.Cells SmartTag");
Console.WriteLine("Initial Deleted value: " + smartTag.Deleted);
// Set the Deleted property to true
smartTag.Deleted = true;
Console.WriteLine("After setting Deleted: " + smartTag.Deleted);
// Save the workbook
workbook.Save("SmartTagDeletedDemo.xlsx");
}
}
}
```
### See Also
* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
