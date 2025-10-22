##FindOptions.SearchNext
FindOptions property. Search order. True search next. False search previous
## FindOptions.SearchNext property
Search order. True: search next. False: search previous.
```csharp
[Obsolete("Use FindOptions.SearchBackward property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SearchNext { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use FindOptions.SearchBackward property. This property will be removed 12 months later since November 2018. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FindOptionsPropertySearchNextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some sample data
worksheet.Cells["A1"].PutValue("Apple");
worksheet.Cells["A2"].PutValue("Banana");
worksheet.Cells["A3"].PutValue("apple");
worksheet.Cells["A4"].PutValue("Orange");
worksheet.Cells["A5"].PutValue("apple pie");
// Create find options
FindOptions findOptions = new FindOptions();
findOptions.CaseSensitive = false;
findOptions.LookAtType = LookAtType.Contains;
// Demonstrate SearchNext property (obsolete, but shown for demonstration)
Console.WriteLine("Initial SearchNext value: " + findOptions.SearchNext);
// Search forward (default behavior)
findOptions.SearchNext = true;
Cell firstForward = worksheet.Cells.Find("apple", null, findOptions);
Console.WriteLine("First forward search result: " + (firstForward != null ? firstForward.Name + " - " + firstForward.StringValue : "Not found"));
// Search backward
findOptions.SearchNext = false;
Cell firstBackward = worksheet.Cells.Find("apple", null, findOptions);
Console.WriteLine("First backward search result: " + (firstBackward != null ? firstBackward.Name + " - " + firstBackward.StringValue : "Not found"));
// Save the workbook
workbook.Save("PropertySearchNextDemo.xlsx");
}
}
}
```
### See Also
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
