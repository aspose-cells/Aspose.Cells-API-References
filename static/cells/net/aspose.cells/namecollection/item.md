##NameCollection.Item
NameCollection property. Gets the Name element at the specified index
## NameCollection indexer (1 of 2)
Gets the [`Name`](../../name/) element at the specified index.
```csharp
public Name this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NameCollectionPropertyItemDemo1
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some worksheets
workbook.Worksheets.Add("Sheet1");
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Access the name collection
NameCollection names = workbook.Worksheets.Names;
// Add named ranges using correct method signature
int index1 = names.Add("Range1");
names[index1].RefersTo = "=Sheet1!$A$1:$B$2";
int index2 = names.Add("Range2");
names[index2].RefersTo = "=Sheet2!$C$3:$D$4";
int index3 = names.Add("Range3");
names[index3].RefersTo = "=Sheet3!$E$5:$F$6";
// Demonstrate Item property usage
Console.WriteLine("Named Ranges:");
for (int i = 0; i < names.Count; i++)
{
Name name = names[i]; // Using Item property with index
Console.WriteLine($"{name.Text}: {name.RefersTo}");
}
// Access by name using Item property
Name specificName = names["Range2"];
Console.WriteLine($"\nSpecific Range: {specificName.Text} refers to {specificName.RefersTo}");
// Modify a named range
names["Range3"].RefersTo = "=Sheet3!$A$1:$B$10";
Console.WriteLine($"\nModified Range3 now refers to: {names["Range3"].RefersTo}");
}
}
}
```
### See Also
* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## NameCollection indexer (2 of 2)
Gets the [`Name`](../../name/) element with the specified name.
```csharp
public Name this[string text] { get; }
```
| Parameter | Description |
| --- | --- |
| text | Name text. |
### Return Value
The element with the specified name.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NameCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the worksheets' names collection
NameCollection names = workbook.Worksheets.Names;
// Add some named ranges (corrected to use proper Add method signature)
int index1 = names.Add("Range1");
names[index1].RefersTo = "=Sheet1!$A$1:$A$10";
int index2 = names.Add("Range2");
names[index2].RefersTo = "=Sheet1!$B$1:$B$10";
// Access named ranges using Item property
Name range1 = names["Range1"];
Name range2 = names["Range2"];
// Verify the names exist
if (range1 != null && range2 != null)
{
Console.WriteLine("Named range 'Range1' refers to: " + range1.RefersTo);
Console.WriteLine("Named range 'Range2' refers to: " + range2.RefersTo);
}
// Try to access a non-existent name
Name range3 = names["NonExistentRange"];
if (range3 == null)
{
Console.WriteLine("Named range 'NonExistentRange' not found");
}
}
}
}
```
### See Also
* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
