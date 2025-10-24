##NameCollection.Add
NameCollection method. Defines a new name
## NameCollection.Add method
Defines a new name.
```csharp
public int Add(string text)
```
| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text to use as the name. |
### Return Value
[`Name`](../../name/) object index.
### Remarks
Name cannot include spaces and cannot look like cell references.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NameCollectionMethodAddWithStringDemo
{
public static void Run()
{
Workbook wb = new Workbook(FileFormatType.Xlsx);
Worksheet worksheet = wb.Worksheets[0];
// Add a name with string reference
int index = wb.Worksheets.Names.Add("MyNamedRange");
Name namedRange = wb.Worksheets.Names[index];
// Set the formula the name refers to
namedRange.RefersTo = "=Sheet1!$A$1:$B$10";
// Verify and output the results
Console.WriteLine("Named Range RefersTo: " + namedRange.RefersTo);
Console.WriteLine("Named Range Index: " + index);
// Get the range and display its address
Aspose.Cells.Range range = namedRange.GetRange();
Console.WriteLine("Range Address: " + range.Address);
}
}
}
```
### See Also
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
