##SmartTagPropertyCollection.Add
SmartTagPropertyCollection method. Adds a property of cells smart tag
## SmartTagPropertyCollection.Add method
Adds a property of cell's smart tag.
```csharp
public int Add(string name, string value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property |
| value | String | The value of the property. |
### Return Value
return [`SmartTagProperty`](../../smarttagproperty/)
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;
namespace AsposeCellsExamples
{
public class SmartTagPropertyCollectionMethodAddWithStringStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
int smartTagIndex = smartTagSetting.Add(0, 0);
SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
smartTags.Add("http://docs.aspose.com", "docs");
SmartTag smartTag = smartTags[0];
SmartTagPropertyCollection properties = smartTag.Properties;
properties.Add("Author", "Aspose");
properties.Add("Version", "1.0");
workbook.Save("SmartTagPropertyDemo.xlsx");
Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
}
}
}
```
### See Also
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
