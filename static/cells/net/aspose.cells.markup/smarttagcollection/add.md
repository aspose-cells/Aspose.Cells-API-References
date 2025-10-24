##SmartTagCollection.Add
SmartTagCollection method. Adds a smart tag
## SmartTagCollection.Add method
Adds a smart tag.
```csharp
public int Add(string uri, string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| uri | String | Specifies the namespace URI of the smart tag |
| name | String | Specifies the name of the smart tag. |
### Return Value
The index of smart tag in the list.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;
namespace AsposeCellsExamples
{
public class SmartTagCollectionMethodAddWithStringStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
smartTagSetting.Add(0, 0); // Add smart tag to cell A1
SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");
Console.WriteLine("Added smart tag at index: " + tagIndex);
workbook.Save("SmartTagCollectionAddExample.xlsx");
}
}
}
```
### See Also
* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
