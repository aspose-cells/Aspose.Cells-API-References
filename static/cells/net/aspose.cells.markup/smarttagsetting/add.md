##SmartTagSetting.Add
SmartTagSetting method. Adds a SmartTagCollection object to a cell
## Add(int, int) {#add}
Adds a [`SmartTagCollection`](../../smarttagcollection/) object to a cell.
```csharp
public int Add(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row of the cell. |
| column | Int32 | The column of the cell. |
### Return Value
Returns index of a [`SmartTagCollection`](../../smarttagcollection/) object in the worksheet.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;
namespace AsposeCellsExamples
{
public class SmartTagSettingMethodAddWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
int smartTagIndex = smartTagSetting.Add(0, 0); // Add to cell A1 (row 0, column 0)
SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");
Console.WriteLine("Smart Tags Count: " + smartTagSetting.Count.ToString());
workbook.Save("SmartTagDemo.xlsx");
}
}
}
```
### See Also
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
## Add(string) {#add_1}
Add a cell smart tags.
```csharp
public int Add(string cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of the cell. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;
public class SmartTagSettingMethodAddWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the SmartTagSetting instance
SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
try
{
// Call the Add method with String parameter
int index = smartTagSetting.Add("A1");
Console.WriteLine($"SmartTag added successfully at index: {index}");
// Add some content to demonstrate the effect
worksheet.Cells["A1"].PutValue("This cell has a smart tag");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the result
workbook.Save("SmartTagSettingMethodAddWithStringDemo.xlsx");
}
}
}
```
### See Also
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
