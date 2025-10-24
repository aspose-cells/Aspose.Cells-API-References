##Class SmartTagSetting
Aspose.Cells.Markup.SmartTagSetting class. Represents all SmartTagCollection object in the worksheet
## SmartTagSetting class
Represents all [`SmartTagCollection`](../smarttagcollection/) object in the worksheet.
```csharp
public class SmartTagSetting : CollectionBase
```
## Properties
| Name | Description |
| --- | --- |
| [Item](../../aspose.cells.markup/smarttagsetting/item/) { get; } | Gets a [`SmartTagCollection`](../smarttagcollection/) object by the index. (3 indexers) |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add_1)(string) | Add a cell smart tags. |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add)(int, int) | Adds a [`SmartTagCollection`](../smarttagcollection/) object to a cell. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;
public class SmartTagSettingDemo
{
public static void SmartTagSettingExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a smart tag to a specific cell
SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
int smartTagIndex = smartTagSetting.Add(0, 0); // Adding smart tag to cell A1
// Access the SmartTagCollection for the cell
SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
// Add a smart tag to the collection
int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");
// Set the capacity of the smart tag setting
smartTagSetting.Capacity = 10;
// Print the count of smart tags
Console.WriteLine("Total Smart Tags: " + smartTagSetting.Count);
// Save the workbook
workbook.Save("SmartTagSettingExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)
