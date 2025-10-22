##NameCollection.Remove
NameCollection method. Remove an array of name
## Remove(string[]) {#remove_1}
Remove an array of name
```csharp
public void Remove(string[] names)
```
| Parameter | Type | Description |
| --- | --- | --- |
| names | String[] | The names' text. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class NameCollectionMethodRemoveWithStringArrayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the NameCollection from the workbook
NameCollection names = workbook.Worksheets.Names;
// Add some named ranges to demonstrate removal
names.Add("TestRange1");
names.Add("TestRange2");
names.Add("TestRange3");
// Prepare the array of names to remove
string[] namesToRemove = new string[] { "TestRange1", "TestRange3" };
try
{
// Call the Remove method with String[] parameter
names.Remove(namesToRemove);
Console.WriteLine("Names removed successfully:");
foreach (string name in namesToRemove)
{
Console.WriteLine(name);
}
// Display remaining names
Console.WriteLine("\nRemaining names in the collection:");
foreach (Name name in names)
{
Console.WriteLine(name.Text);
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Remove method: {ex.Message}");
}
// Save the result
workbook.Save("NameCollectionRemoveDemo.xlsx");
}
}
}
```
### See Also
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Remove(string) {#remove}
Remove the name.
```csharp
public void Remove(string text)
```
| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The name text. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NameCollectionMethodRemoveWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add a named range
Aspose.Cells.Range range = sheet.Cells.CreateRange("A1", "B10");
range.Name = "TestRange";
// Display count before removal
Console.WriteLine("Named ranges count before removal: " + workbook.Worksheets.Names.Count);
// Remove the named range
workbook.Worksheets.Names.Remove("TestRange");
// Display count after removal
Console.WriteLine("Named ranges count after removal: " + workbook.Worksheets.Names.Count);
}
}
}
```
### See Also
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
