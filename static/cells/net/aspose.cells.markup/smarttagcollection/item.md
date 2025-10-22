##SmartTagCollection.Item
SmartTagCollection property. Gets a SmartTag object at the specific index
## SmartTagCollection indexer
Gets a [`SmartTag`](../../smarttag/) object at the specific index
```csharp
public SmartTag this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Return Value
returns a [`SmartTag`](../../smarttag/) object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;
namespace AsposeCellsExamples
{
public class SmartTagCollectionPropertyItemDemo
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
// Demonstrate Item property usage
SmartTagProperty authorProperty = properties["Author"];
Console.WriteLine($"Property 'Author' value: {authorProperty.Value}");
workbook.Save("SmartTagPropertyDemo.xlsx");
Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
}
}
}
```
### See Also
* class [SmartTag](../../smarttag/)
* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
