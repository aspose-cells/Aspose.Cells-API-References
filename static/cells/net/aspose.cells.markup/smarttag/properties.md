##SmartTag.Properties
SmartTag property. Gets and set the properties of the smart tag
## SmartTag.Properties property
Gets and set the properties of the smart tag.
```csharp
public SmartTagPropertyCollection Properties { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;
namespace AsposeCellsExamples
{
public class SmartTagPropertyPropertiesDemo
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
properties.Add("Author", "John Doe");
properties.Add("Version", "1.0");
properties.Add("Category", "Demo");
Console.WriteLine("Smart Tag Properties:");
foreach (SmartTagProperty prop in properties)
{
Console.WriteLine($"{prop.Name}: {prop.Value}");
}
workbook.Save("SmartTagPropertiesDemo.xlsx");
}
}
}
```
### See Also
* class [SmartTagPropertyCollection](../../smarttagpropertycollection/)
* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
