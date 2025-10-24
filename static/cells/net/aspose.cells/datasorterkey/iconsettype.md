##DataSorterKey.IconSetType
DataSorterKey property. Represents the icon set type
## DataSorterKey.IconSetType property
Represents the icon set type.
```csharp
public IconSetType IconSetType { get; }
```
### Remarks
Only takes effect when [`Type`](../type/) is Icon.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterKeyPropertyIconSetTypeDemo
{
public static void Run()
{
// Create a workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with icon set conditional formatting
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
worksheet.Cells["A5"].PutValue(50);
// Add icon set conditional formatting
ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
int index = cfc.Add();
FormatConditionCollection fcc = cfc[index];
CellArea area = CellArea.CreateCellArea("A1", "A5");
fcc.AddArea(area);
fcc.AddCondition(FormatConditionType.IconSet);
fcc[0].IconSet.Type = IconSetType.Arrows3;
// Create data sorter with icon set type
DataSorter sorter = workbook.DataSorter;
sorter.AddKey(0, SortOrder.Ascending);
// Sort the data
sorter.Sort(worksheet.Cells, area);
// Display the icon set type from the sorter key
foreach (DataSorterKey key in sorter.Keys)
{
Console.WriteLine($"IconSetType used for sorting: {key.IconSetType}");
}
// Save the workbook
workbook.Save("IconSetTypeSortingDemo.xlsx");
}
}
}
```
### See Also
* enum [IconSetType](../../iconsettype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
