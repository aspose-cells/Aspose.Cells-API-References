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
// Called: PivotConditionalFormatCollection pfcc = table.ConditionalFormats;
[Test]
        public void Type_PivotConditionalFormatCollection()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;JAVA42247_&quot;;
            Workbook book = new Workbook(filePath + &quot;Coalition_Advance_Cross_Tab_05042017_1102.xlsx&quot;);
            Worksheet sheet2 = book.Worksheets[&quot;Advanced CrossTab&quot;];
            PivotTable table = book.Worksheets[&quot;Advanced CrossTab&quot;].PivotTables[0];
            table.RefreshData();
            table.CalculateData();
            table.RefreshDataOnOpeningFile = false;

            PivotConditionalFormatCollection pfcc = table.ConditionalFormats;
            int pIndex = pfcc.Add();
            PivotConditionalFormat pfc = pfcc[pIndex];
            FormatConditionCollection fcc = pfc.FormatConditions;
            CellArea dataBodyRange = table.DataBodyRange;
            fcc.AddArea(dataBodyRange);
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = &quot;224&quot;;
            fc.Operator = OperatorType.Equal;
            fc.Text = &quot;NA&quot;;
            fc.Style.BackgroundColor = Color.Red;

            //sheet 上的条件格式，在透视表自动刷新后会被覆盖掉，需要用透视表的条件格式才行
            //ConditionalFormattingCollection cfs = sheet2.ConditionalFormattings;
            //int index123 = cfs.Add();
            //FormatConditionCollection fcs = cfs[index123];
            //CellArea dataBodyRange = table.DataBodyRange;
            ////ca = new CellArea();
            //fcs.AddArea(dataBodyRange);//geting all body of pivot values here
            //int idx = fcs.AddCondition(FormatConditionType.CellValue);
            //FormatCondition fc = fcs[idx];
            //fc.Formula1 = &quot;224&quot;;
            //fc.Operator = OperatorType.Equal;
            //fc.Text = &quot;NA&quot;;
            //fc.Style.BackgroundColor = Color.Red;



            book.Save(CreateFolder(filePath) + &quot;outout.xlsx&quot;);
        }
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotConditionalFormat](../pivotconditionalformat/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


