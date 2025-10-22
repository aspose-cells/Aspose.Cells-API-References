##SmartTagSetting.Item
SmartTagSetting property. Gets a SmartTagCollection object by the index
## SmartTagSetting indexer (1 of 3)
Gets a [`SmartTagCollection`](../../smarttagcollection/) object by the index.
```csharp
public SmartTagCollection this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index of the [`SmartTagCollection`](../../smarttagcollection/) object in the list. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;
namespace AsposeCellsExamples
{
public class SmartTagSettingPropertyItemDemo1
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Aspose");
sheet.Cells["A2"].PutValue("Cells");
SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
int smartTagIndex = smartTagSetting.Add(0, 0);
// Demonstrate Item property usage
SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
smartTags.Add("http://docs.aspose.com", "docs");
SmartTag smartTag = smartTags[0];
smartTag.SetLink("http://www.aspose.com", "AsposeLink");
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
* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
## SmartTagSetting indexer (2 of 3)
Gets the [`SmartTagCollection`](../../smarttagcollection/) object of the cell.
```csharp
public SmartTagCollection this[int row, int column] { get; }
```
| Parameter | Description |
| --- | --- |
| row | The row index of the cell. |
| column | The column index of the cell |
### Return Value
Returns the [`SmartTagCollection`](../../smarttagcollection/) object of the cell. Returns null if there is no any smart tags on the cell.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;
namespace AsposeCellsExamples
{
public class SmartTagSettingPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
smartTagSetting.Add(0, 0); // Add smart tag to cell A1
// Demonstrate Item property usage
SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");
Console.WriteLine("Smart tags in cell A1: " + smartTagCollection.Count);
Console.WriteLine("Namespace URI: " + smartTagCollection[0].Uri);
Console.WriteLine("Tag name: " + smartTagCollection[0].Name);
workbook.Save("SmartTagDemo.xlsx");
}
}
}
```
### See Also
* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
## SmartTagSetting indexer (3 of 3)
Gets the [`SmartTagCollection`](../../smarttagcollection/) object of the cell.
```csharp
public SmartTagCollection this[string cellName] { get; }
```
| Parameter | Description |
| --- | --- |
| cellName | The name of the cell. |
### Return Value
Returns the [`SmartTagCollection`](../../smarttagcollection/) object of the cell. Returns null if there is no any smart tags on the cell.
### See Also
* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
