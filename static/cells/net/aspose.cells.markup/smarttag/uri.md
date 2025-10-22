##SmartTag.Uri
SmartTag property. Gets the namespace URI of the smart tag
## SmartTag.Uri property
Gets the namespace URI of the smart tag.
```csharp
public string Uri { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;
public class SmartTagPropertyUriDemo
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
// Display the Uri property value (read-only operation)
Console.WriteLine("SmartTag Uri: " + smartTag.Uri);
// Demonstrate other properties
Console.WriteLine("SmartTag Name: " + smartTag.Name);
// Save the workbook
workbook.Save("SmartTagUriDemo.xlsx");
}
}
}
```
### See Also
* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
