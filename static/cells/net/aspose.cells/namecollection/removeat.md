##NameCollection.RemoveAt
NameCollection method. Remove the name at the specific index
## NameCollection.RemoveAt method
Remove the name at the specific index.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | index of the Name to be removed. |
### Remarks
Please make sure that the name is not referred by the other formulas before calling the method. And if the name is referred, setting Name.RefersTo as null is better.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NameCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
WorksheetCollection worksheets = workbook.Worksheets;
NameCollection names = worksheets.Names;
// Add names to the collection
int firstIndex = names.Add("FirstRange");
names[firstIndex].RefersTo = "=Sheet1!$A$1:$A$5";
int secondIndex = names.Add("SecondRange");
names[secondIndex].RefersTo = "=Sheet1!$B$1:$B$5";
// Remove name by index
names.RemoveAt(firstIndex);
// Verify removal by checking count
Console.WriteLine($"Remaining names count: {names.Count}");
workbook.Save("NameCollectionRemoveAtExample.xlsx");
}
}
}
```
### See Also
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
