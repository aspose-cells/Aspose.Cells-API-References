##ListObjectCollection.Item
ListObjectCollection property. Gets the ListObject by index
## ListObjectCollection indexer (1 of 2)
Gets the ListObject by index.
```csharp
public ListObject this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Return Value
The ListObject
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectCollectionPropertyItemDemo1
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create a list object
int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject listObject = worksheet.ListObjects[index];
// Access list object using Item property
ListObject firstListObject = worksheet.ListObjects[0];
// Set table style
firstListObject.TableStyleType = TableStyleType.TableStyleMedium2;
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
## ListObjectCollection indexer (2 of 2)
Gets the ListObject by specified name.
```csharp
public ListObject this[string tableName] { get; }
```
| Parameter | Description |
| --- | --- |
| tableName | ListObject name. |
### Return Value
The ListObject
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create a list object
int index = worksheet.ListObjects.Add("A1", "B3", true);
ListObject listObj = worksheet.ListObjects[index];
listObj.DisplayName = "PersonTable";
// Access the list object using Item property by name
ListObject retrievedListObj = worksheet.ListObjects["PersonTable"];
// Demonstrate usage by converting to range
retrievedListObj.ConvertToRange();
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
