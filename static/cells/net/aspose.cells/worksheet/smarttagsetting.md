##Worksheet.SmartTagSetting
Worksheet property. Gets all SmartTagCollection objects of the worksheet
## Worksheet.SmartTagSetting property
Gets all [`SmartTagCollection`](../../../aspose.cells.markup/smarttagcollection/) objects of the worksheet.
```csharp
public SmartTagSetting SmartTagSetting { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;
namespace AsposeCellsExamples
{
public class WorksheetPropertySmartTagSettingDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
int smartTagIndex = smartTagSetting.Add(0, 0);
SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");
Console.WriteLine("Smart Tags Count: " + smartTagSetting.Count.ToString());
workbook.Save("SmartTagSettingDemo.xlsx");
}
}
}
```
### See Also
* class [SmartTagSetting](../../../aspose.cells.markup/smarttagsetting/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
