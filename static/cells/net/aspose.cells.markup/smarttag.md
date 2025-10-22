##Class SmartTag
Aspose.Cells.Markup.SmartTag class. Represents a smart tag
## SmartTag class
Represents a smart tag.
```csharp
public class SmartTag
```
## Properties
| Name | Description |
| --- | --- |
| [Deleted](../../aspose.cells.markup/smarttag/deleted/) { get; set; } | Indicates whether the smart tag is deleted. |
| [Name](../../aspose.cells.markup/smarttag/name/) { get; } | Gets the name of the smart tag. |
| [Properties](../../aspose.cells.markup/smarttag/properties/) { get; set; } | Gets and set the properties of the smart tag. |
| [Uri](../../aspose.cells.markup/smarttag/uri/) { get; } | Gets the namespace URI of the smart tag. |
## Methods
| Name | Description |
| --- | --- |
| [SetLink](../../aspose.cells.markup/smarttag/setlink/)(string, string) | Change the name and the namespace URI of the smart tag. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;
namespace AsposeCellsExamples
{
public class MarkupClassSmartTagDemo
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
workbook.Save("SmartTagDemo.xlsx");
Console.WriteLine("SmartTagDemo.xlsx created successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)
