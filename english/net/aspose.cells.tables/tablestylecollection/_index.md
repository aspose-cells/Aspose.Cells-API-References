---
title: Class TableStyleCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Tables.TableStyleCollection class. Represents all custom table styles
type: docs
url: /net/aspose.cells.tables/tablestylecollection/
---
## TableStyleCollection class

Represents all custom table styles.

```csharp
public class TableStyleCollection : CollectionBase<TableStyle>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [DefaultPivotStyleName](../../aspose.cells.tables/tablestylecollection/defaultpivotstylename/) { get; set; } | Gets and sets the default style name of pivot table . |
| [DefaultTableStyleName](../../aspose.cells.tables/tablestylecollection/defaulttablestylename/) { get; set; } | Gets and sets the default style name of the table. |
| [Item](../../aspose.cells.tables/tablestylecollection/item/) { get; } | Gets the table style by the index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [AddPivotTableStyle](../../aspose.cells.tables/tablestylecollection/addpivottablestyle/)(string) | Adds a custom pivot table style. |
| [AddTableStyle](../../aspose.cells.tables/tablestylecollection/addtablestyle/)(string) | Adds a custom table style. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyle) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyle, IComparer&lt;TableStyle&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, TableStyle, IComparer&lt;TableStyle&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(TableStyle) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyle[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyle[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, TableStyle[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;TableStyle&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;TableStyle&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;TableStyle&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;TableStyle&gt;) |  |
| [GetBuiltinTableStyle](../../aspose.cells.tables/tablestylecollection/getbuiltintablestyle/)(TableStyleType) | Gets the builtin table style |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
// Called: TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
public void Tables_Type_TableStyleCollection()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
    Assert.AreEqual("TableStyleDark3", tableStyles.DefaultTableStyleName);
    Assert.AreEqual("PivotStyleLight16", tableStyles.DefaultPivotStyleName);

    tableStyles.DefaultTableStyleName = "TableStyleMedium9";
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    tableStyles = workbook.Worksheets.TableStyles;
    Assert.AreEqual("TableStyleMedium9", tableStyles.DefaultTableStyleName);
}
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TableStyle](../tablestyle/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


