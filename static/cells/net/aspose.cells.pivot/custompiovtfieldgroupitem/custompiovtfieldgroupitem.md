##CustomPiovtFieldGroupItem.CustomPiovtFieldGroupItem
CustomPiovtFieldGroupItem constructor. The constructor of custom group item of pivot field
## CustomPiovtFieldGroupItem constructor
The constructor of custom group item of pivot field.
```csharp
public CustomPiovtFieldGroupItem(string name, int[] itemIndexes)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of group item |
| itemIndexes | Int32[] | All indexes to the items of base pivot field. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.Pivot;
using System;
public class CustomPiovtFieldGroupItemMethodCtorWithStringInt32ArrayDemo
{
public static void Run()
{
try
{
// Create a custom pivot field group item with name and item indexes
string groupName = "AgeGroup";
int[] itemIndexes = { 1, 2, 3 }; // Example indexes for grouped items
// Call the constructor with String and Int32[] parameters
var customGroupItem = new CustomPiovtFieldGroupItem(groupName, itemIndexes);
Console.WriteLine("CustomPiovtFieldGroupItem created successfully with:");
Console.WriteLine($"Group Name: {groupName}");
Console.WriteLine($"Item Indexes: {string.Join(", ", itemIndexes)}");
}
catch (Exception ex)
{
Console.WriteLine($"Error creating CustomPiovtFieldGroupItem: {ex.Message}");
}
}
}
}
```
### See Also
* class [CustomPiovtFieldGroupItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
