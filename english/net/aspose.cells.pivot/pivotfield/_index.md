---
title: Class PivotField
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotField class. Represents a field in a PivotTable report
type: docs
url: /net/aspose.cells.pivot/pivotfield/
---
## PivotField class

Represents a field in a PivotTable report.

```csharp
public class PivotField
```

## Properties

| Name | Description |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount/) { get; set; } | Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield/) { get; set; } | Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields. |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield/) { get; set; } | Represents auto sort field index. -1 means PivotField itself,others means the position of the data fields. |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotfield/basefieldindex/) { get; set; } | Represents the base field for a custom calculation. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex/) { get; set; } | Represents the PivotField index in the base PivotFields. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotfield/baseitemindex/) { get; set; } | Represents the item in the base field for a custom calculation. Valid only for data fields. |
| [BaseItemPosition](../../aspose.cells.pivot/pivotfield/baseitemposition/) { get; set; } | Represents the item in the base field for a custom calculation. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem/) { get; set; } | Represents the current page item showing for the page field (valid only for page fields). |
| [DataDisplayFormat](../../aspose.cells.pivot/pivotfield/datadisplayformat/) { get; set; } | Represents how to display the values contained in a data field. |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname/) { get; set; } | Represents the PivotField display name. |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn/) { get; set; } | Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata/) { get; set; } | Indicates whether the specified field can be dragged to the data position. The default value is true. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide/) { get; set; } | Indicates whether the specified field can be dragged to the hide position. The default value is true. |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage/) { get; set; } | Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow/) { get; set; } | Indicates whether the specified field can be dragged to the row position. The default value is true. |
| [Function](../../aspose.cells.pivot/pivotfield/function/) { get; set; } | Represents the function used to summarize the PivotTable data field. |
| [GroupSettings](../../aspose.cells.pivot/pivotfield/groupsettings/) { get; } | Gets the group settings of the pivot field. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow/) { get; set; } | Indicates whether inserting blank line after each item. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow/) { get; set; } | Indicates whether the specified PivotTable field is autoshown ascending. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort/) { get; set; } | Indicates whether the specified PivotTable field is autosorted ascending. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow/) { get; set; } | Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort/) { get; set; } | Indicates whether the specified PivotTable field is automatically sorted. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals/) { get; set; } | Indicates whether the specified field shows automatic subtotals. Default is true. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield/) { get; } | Indicates whether the specified PivotTable field is calculated field. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter/) { get; set; } | indicates whether the field can include new items in manual filter The default value is false. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems/) { get; set; } | indicates whether the field can insert page breaks between items insert page break after each item The default value is false. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed/) { get; set; } | indicates whether the field can have multiple items selected in the page field The default value is false. |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels/) { get; set; } | indicates whether the field can repeat items labels The default value is false. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount/) { get; } | Gets the base item count of this pivot field. |
| [Items](../../aspose.cells.pivot/pivotfield/items/) { get; } | Get all base items; |
| [Name](../../aspose.cells.pivot/pivotfield/name/) { get; set; } | Represents the PivotField name. |
| [NonAutoSortDefault](../../aspose.cells.pivot/pivotfield/nonautosortdefault/) { get; set; } | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [Number](../../aspose.cells.pivot/pivotfield/number/) { get; set; } | Represents the built-in display format of numbers and dates. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat/) { get; set; } | Represents the custom display format of numbers and dates. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems/) { get; } | Get the original base items; |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems/) { get; } | Gets the pivot items of the pivot field |
| [Position](../../aspose.cells.pivot/pivotfield/position/) { get; } | Represents the PivotField index in the PivotFields. |
| [Range](../../aspose.cells.pivot/pivotfield/range/) { get; } | (**Obsolete.**) Gets the group range of the pivot field |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems/) { get; set; } | Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact/) { get; set; } | Indicates whether display labels from the next field in the same column on the Pivot Table view |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform/) { get; set; } | Indicates whether layout this field in outline form on the Pivot Table view |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop/) { get; set; } | when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |

## Methods

| Name | Description |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem/)(string, string) | Add a calculated item to the pivot field. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula/)() | Get the formula string of the specified calculated field . |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype/)(PivotFilterType) | Gets the pivot filter of the pivot field by type |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters/)() | Gets the pivot filters of the pivot field |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals/)(PivotFieldSubtotalType) | Gets whether the specified field shows that subtotals. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby)(CustomPiovtFieldGroupItem[], bool) | Custom group the field. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_1)(double, double, double, bool) | Group the file by number. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_2)(DateTime, DateTime, PivotGroupByType[], double, bool) | Group the file by the date group types. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail/)(bool) | Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem/#hideitem)(int, bool) | Sets whether the specific PivotItem in a data field is hidden. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem/#hideitem_1)(string, bool) | Sets whether the specific PivotItem in a data field is hidden. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail/)(int, bool) | Sets whether the specific PivotItem in a pivot field is hidden detail. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems/)() | Init the pivot items of the pivot field |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem/)(int) | Indicates whether the specific PivotItem is hidden. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail/)(int) | Indicates whether the specific PivotItem is hidden detail. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals/)(PivotFieldSubtotalType, bool) | Sets whether the specified field shows that subtotals. |
| [Ungroup](../../aspose.cells.pivot/pivotfield/ungroup/)() | Ungroup the pivot field. |

### Examples

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Change PivotField's attributes
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

pivot.RefreshData();
pivot.CalculateData();

//do your business

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


