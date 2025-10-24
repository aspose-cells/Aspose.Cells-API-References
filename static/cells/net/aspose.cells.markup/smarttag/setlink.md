##SmartTag.SetLink
SmartTag method. Change the name and the namespace URI of the smart tag
## SmartTag.SetLink method
Change the name and the namespace URI of the smart tag.
```csharp
public void SetLink(string uri, string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| uri | String | The namespace URI of the smart tag. |
| name | String | The name of the smart tag. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;
namespace AsposeCellsExamples
{
public class SmartTagMethodSetLinkWithStringStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Aspose");
SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
int smartTagIndex = smartTagSetting.Add(0, 0);
SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
smartTags.Add("http://docs.aspose.com", "docs");
SmartTag smartTag = smartTags[0];
smartTag.SetLink("http://www.aspose.com", "AsposeLink");
workbook.Save("SmartTagSetLinkDemo.xlsx");
}
}
}
```
### See Also
* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
