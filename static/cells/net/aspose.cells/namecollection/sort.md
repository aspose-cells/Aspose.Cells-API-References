##NameCollection.Sort
NameCollection method. Sorts defined names
## NameCollection.Sort method
Sorts defined names.
```csharp
public void Sort()
```
### Remarks
If you create a large amount of named ranges in the Excel file, please call this method after all named ranges are created and before saving
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class NameCollectionMethodSortDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the NameCollection from the workbook
NameCollection names = workbook.Worksheets.Names;
// Add some named ranges to demonstrate sorting
names.Add("RangeC");
names.Add("RangeA");
names.Add("RangeB");
try
{
// Display names before sorting
Console.WriteLine("Names before sorting:");
foreach (Name name in names)
{
Console.WriteLine(name.Text);
}
// Call the Sort method
names.Sort();
// Display names after sorting
Console.WriteLine("\nNames after sorting:");
foreach (Name name in names)
{
Console.WriteLine(name.Text);
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Sort method: {ex.Message}");
}
// Save the result
workbook.Save("NameCollectionSortDemo.xlsx");
}
}
}
```
### See Also
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
