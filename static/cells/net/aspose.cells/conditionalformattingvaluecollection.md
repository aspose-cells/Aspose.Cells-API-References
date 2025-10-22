##Class ConditionalFormattingValueCollection
Aspose.Cells.ConditionalFormattingValueCollection class. Describes a collection of CFValueObject. Use only for icon sets
## ConditionalFormattingValueCollection class
Describes a collection of CFValueObject. Use only for icon sets.
```csharp
public class ConditionalFormattingValueCollection : CollectionBase<ConditionalFormattingValue>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingvaluecollection/item/) { get; } | Get the CFValueObject element at the specified index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingvaluecollection/add/)(FormatConditionValueType, string) | Adds [`ConditionalFormattingValue`](../conditionalformattingvalue/) object. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConditionalFormattingValue) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConditionalFormattingValue, IComparer&lt;ConditionalFormattingValue&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ConditionalFormattingValue, IComparer&lt;ConditionalFormattingValue&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ConditionalFormattingValue) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConditionalFormattingValue[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConditionalFormattingValue[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ConditionalFormattingValue[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingValue) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingValue, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingValue, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingValue) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingValue, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingValue, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ConditionalFormattingValueCollectionDemo
{
public static void ConditionalFormattingValueCollectionExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Adds an empty conditional formatting
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
// Sets the conditional format range
CellArea ca = new CellArea
{
StartRow = 0,
EndRow = 2,
StartColumn = 0,
EndColumn = 0
};
fcs.AddArea(ca);
// Adds condition
int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
FormatCondition cond = fcs[conditionIndex];
// Get Icon Set
IconSet iconSet = cond.IconSet;
// Set Icon Type
iconSet.Type = IconSetType.Arrows3;
// Get the CFValueObjects instance
ConditionalFormattingValueCollection cfvos = iconSet.Cfvos;
// Add a new ConditionalFormattingValue to the collection
int cfvIndex = cfvos.Add(FormatConditionValueType.Number, "50");
// Access the newly added ConditionalFormattingValue
ConditionalFormattingValue cfv = cfvos[cfvIndex];
// Modify properties of the ConditionalFormattingValue
cfv.Value = 75;
cfv.Type = FormatConditionValueType.Percent;
cfv.IsGTE = true;
// Put Cell Values
sheet.Cells["A1"].PutValue(10);
sheet.Cells["A2"].PutValue(120);
sheet.Cells["A3"].PutValue(260);
// Saving the Excel file
workbook.Save("ConditionalFormattingValueCollectionExample.xlsx");
workbook.Save("ConditionalFormattingValueCollectionExample.pdf");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ConditionalFormattingValue](../conditionalformattingvalue/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
