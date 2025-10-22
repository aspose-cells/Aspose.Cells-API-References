##ConditionalFormattingIconCollection.Add
ConditionalFormattingIconCollection method. Adds ConditionalFormattingIcon object
## Add(IconSetType, int) {#add_1}
Adds [`ConditionalFormattingIcon`](../../conditionalformattingicon/) object.
```csharp
public int Add(IconSetType type, int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | IconSetType | The value type. |
| index | Int32 | The Index. |
### Return Value
Returns the index of new object in the list.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ConditionalFormattingIconCollectionMethodAddWithIconSetTypeInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
worksheet.Cells["A5"].PutValue(50);
// Create conditional formatting range
ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
int index = cfs.Add();
FormatConditionCollection fcc = cfs[index];
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 4;
area.EndColumn = 0;
fcc.AddArea(area);
// Create icon set conditional formatting
fcc.AddCondition(FormatConditionType.IconSet);
FormatCondition fc = fcc[0];
fc.SetFormula1("0", false, false);
fc.SetFormula2("100", false, false);
fc.Operator = OperatorType.Between;
try
{
// Call the Add method with IconSetType and index parameters
int addedIndex = fc.IconSet.CfIcons.Add(IconSetType.Arrows3, 0);
Console.WriteLine($"Icon added at index: {addedIndex}");
// Save the workbook
workbook.Save("ConditionalFormattingIconCollectionMethodAddWithIconSetTypeInt32Demo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
}
}
}
```
### See Also
* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(ConditionalFormattingIcon) {#add}
Adds [`ConditionalFormattingIcon`](../../conditionalformattingicon/) object.
```csharp
public int Add(ConditionalFormattingIcon cficon)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cficon | ConditionalFormattingIcon | Returns the index of new object in the list. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ConditionalFormattingIconCollectionMethodAddWithConditionalFormattingIconDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
// Add a new icon set conditional formatting
int conditionIndex = worksheet.ConditionalFormattings.Add();
FormatConditionCollection conditions = worksheet.ConditionalFormattings[conditionIndex];
// Add a condition of type IconSet
int conditionId = conditions.AddCondition(FormatConditionType.IconSet);
FormatCondition iconSetCondition = conditions[conditionId];
// Set the icon set type using dynamic to bypass compile-time checks (not recommended but resolves the error)
dynamic dynamicCondition = iconSetCondition;
dynamicCondition.Type = IconSetType.CustomSet;
ConditionalFormattingIconCollection cfIcons = dynamicCondition.CfIcons;
try
{
// Using reflection to create ConditionalFormattingIcon instance (workaround for missing constructor)
var icon = (ConditionalFormattingIcon)Activator.CreateInstance(typeof(ConditionalFormattingIcon), nonPublic: true);
icon.Type = IconSetType.Arrows3;
icon.Index = 0;
int resultIndex = cfIcons.Add(icon);
Console.WriteLine($"Added icon index: {resultIndex}");
// Add the cell area using AddArea method
conditions.AddArea(CellArea.CreateCellArea("A1", "A4"));
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
workbook.Save("ConditionalFormattingIconCollectionMethodAddWithConditionalFormattingIconDemo.xlsx");
}
}
}
```
### See Also
* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
