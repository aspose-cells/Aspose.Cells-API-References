##NameCollection.RemoveDuplicateNames
NameCollection method. Remove the duplicate defined names
## NameCollection.RemoveDuplicateNames method
Remove the duplicate defined names
```csharp
public void RemoveDuplicateNames()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NameCollectionMethodRemoveDuplicateNamesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some named ranges with duplicate names
worksheet.Cells["A1"].PutValue("Test Value 1");
worksheet.Cells["B1"].PutValue("Test Value 2");
// Create duplicate named ranges using the correct Add method signature
int index1 = workbook.Worksheets.Names.Add("DuplicateName");
workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
int index2 = workbook.Worksheets.Names.Add("DuplicateName");
workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$B$1";
// Display count before removing duplicates
Console.WriteLine($"Named ranges count before removal: {workbook.Worksheets.Names.Count}");
// Remove duplicate names
workbook.Worksheets.Names.RemoveDuplicateNames();
// Display count after removing duplicates
Console.WriteLine($"Named ranges count after removal: {workbook.Worksheets.Names.Count}");
}
}
}
```
### See Also
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
