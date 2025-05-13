---
title: Class PivotConditionalFormatCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotConditionalFormatCollection class. Represents all conditional formats of pivot table
type: docs
url: /net/aspose.cells.pivot/pivotconditionalformatcollection/
---
## PivotConditionalFormatCollection class

Represents all conditional formats of pivot table.

```csharp
public class PivotConditionalFormatCollection : CollectionBase<PivotConditionalFormat>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotconditionalformatcollection/item/) { get; } | Gets the pivot FormatCondition object at the specific index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivotconditionalformatcollection/add/)() | Adds a pivot FormatCondition to the collection. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotConditionalFormat) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotConditionalFormat, IComparer&lt;PivotConditionalFormat&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotConditionalFormat, IComparer&lt;PivotConditionalFormat&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotConditionalFormat) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotConditionalFormat[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotConditionalFormat[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotConditionalFormat[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotConditionalFormat&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotConditionalFormat) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotConditionalFormat, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotConditionalFormat, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotConditionalFormat) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotConditionalFormat, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotConditionalFormat, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
// Called: PivotConditionalFormatCollection pfcc = pivot.ConditionalFormats;
public void Pivot_Type_PivotConditionalFormatCollection()
{
    string filePath = Constants.PivotTableSourcePath + @"NET47335_";

    Workbook workbook = new Workbook(filePath + "Filter.xlsx");
    PivotTable table = workbook.Worksheets[0].PivotTables[0];
    PivotField pivotField = table.PageFields[0];

    pivotField.IsMultipleItemSelectionAllowed = true;

    int pageItemCount = pivotField.PivotItems.Count;
    //Select a, e, i, oitems only 
    for (int i = 0; i < pageItemCount; i++)
    {
        PivotItem item = pivotField.PivotItems[i];
        switch (item.Name)
        {
            case "a":
            case "e":
            case "i":
            case "o":
                item.IsHidden = false;
                break;
            default:
                item.IsHidden = true;
                break;
        }
    }

    table.RefreshData();
    table.CalculateData();

    workbook.Save(CreateFolder(filePath) + "filter_out.xlsx");

    Workbook wb = new Workbook(filePath + "To Aspose.xlsx");
    Worksheet sheet = wb.Worksheets.Add("Test");
    int pivotIndex = sheet.PivotTables.Add("=ExportPOC2_AggregateData7_M!$A$1:$D$24", "A3", "TestPivot");
    PivotTable pivot = sheet.PivotTables[pivotIndex];
    pivot.AddFieldToArea(PivotFieldType.Row, 0);
    pivot.AddFieldToArea(PivotFieldType.Column, 1);
    pivot.AddFieldToArea(PivotFieldType.Data, 3);

    pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight16;

    pivot.RefreshData();
    pivot.CalculateData();

    PivotConditionalFormatCollection pfcc = pivot.ConditionalFormats;
    int pIndex = pfcc.Add();
    PivotConditionalFormat pfc = pfcc[pIndex];
    FormatConditionCollection fcc = pfc.FormatConditions;
    CellArea dataBodyRange = pivot.DataBodyRange;

    string startCell = CellsHelper.CellIndexToName(dataBodyRange.StartRow, dataBodyRange.StartColumn);
    fcc.AddArea(dataBodyRange);

    //you can add other format conditions
    //now we will replace 1 with "Direct"
    int idx = fcc.AddCondition(FormatConditionType.Expression);
    FormatCondition fc = fcc[idx];
    fc.Formula1 = "=" + startCell + "=1";
    fc.Operator = OperatorType.Equal;
    fc.Style.Custom = "[=1]\"Direct\";;";

    //replace 8 with "Direct8"
    idx = fcc.AddCondition(FormatConditionType.Expression);
    fc = fcc[idx];
    fc.Formula1 = "=" + startCell + "=8";
    fc.Operator = OperatorType.Equal;
    fc.Style.Custom = "[=8]\"Direct8\";;";


    wb.Save(CreateFolder(filePath) + "ToAspose_out.xlsx");
}
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotConditionalFormat](../pivotconditionalformat/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


