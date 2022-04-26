---
title: PivotField
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 4500
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
| [AutoShowCount](autoshowcount) { get; set; } | Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [AutoShowField](autoshowfield) { get; set; } | Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields. |
| [AutoSortField](autosortfield) { get; set; } | Represents auto sort field index. -1 means PivotField itself,others means the position of the data fields. |
| [BaseFieldIndex](basefieldindex) { get; set; } | Represents the base field for a custom calculation. |
| [BaseIndex](baseindex) { get; set; } | Represents the PivotField index in the base PivotFields. |
| [BaseItemIndex](baseitemindex) { get; set; } | Represents the item in the base field for a custom calculation. Valid only for data fields. |
| [BaseItemPosition](baseitemposition) { get; set; } | Represents the item in the base field for a custom calculation. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [CurrentPageItem](currentpageitem) { get; set; } | Represents the current page item showing for the page field (valid only for page fields). |
| [DataDisplayFormat](datadisplayformat) { get; set; } | Represents how to display the values contained in a data field. |
| [DisplayName](displayname) { get; set; } | Represents the PivotField display name. |
| [DragToColumn](dragtocolumn) { get; set; } | Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [DragToData](dragtodata) { get; set; } | Indicates whether the specified field can be dragged to the data position. The default value is true. |
| [DragToHide](dragtohide) { get; set; } | Indicates whether the specified field can be dragged to the hide position. The default value is true. |
| [DragToPage](dragtopage) { get; set; } | Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [DragToRow](dragtorow) { get; set; } | Indicates whether the specified field can be dragged to the row position. The default value is true. |
| [Function](function) { get; set; } | Represents the function used to summarize the PivotTable data field. |
| [InsertBlankRow](insertblankrow) { get; set; } | Indicates whether inserting blank line after each item. |
| [IsAscendShow](isascendshow) { get; set; } | Indicates whether the specified PivotTable field is autoshown ascending. |
| [IsAscendSort](isascendsort) { get; set; } | Indicates whether the specified PivotTable field is autosorted ascending. |
| [IsAutoShow](isautoshow) { get; set; } | Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
| [IsAutoSort](isautosort) { get; set; } | Indicates whether the specified PivotTable field is automatically sorted. |
| [IsAutoSubtotals](isautosubtotals) { get; set; } | Indicates whether the specified field shows automatic subtotals. Default is true. |
| [IsCalculatedField](iscalculatedfield) { get; } | Indicates whether the specified PivotTable field is calculated field. |
| [IsIncludeNewItemsInFilter](isincludenewitemsinfilter) { get; set; } | indicates whether the field can include new items in manual filter The default value is false. |
| [IsInsertPageBreaksBetweenItems](isinsertpagebreaksbetweenitems) { get; set; } | indicates whether the field can insert page breaks between items insert page break after each item The default value is false. |
| [IsMultipleItemSelectionAllowed](ismultipleitemselectionallowed) { get; set; } | indicates whether the field can have multiple items selected in the page field The default value is false. |
| [IsRepeatItemLabels](isrepeatitemlabels) { get; set; } | indicates whether the field can repeat items labels The default value is false. |
| [ItemCount](itemcount) { get; } | Gets the base item count of this pivot field. |
| [Items](items) { get; } | Get all base items; |
| [Name](name) { get; } | Represents the PivotField name. |
| [Number](number) { get; set; } | Represents the built-in display format of numbers and dates. |
| [NumberFormat](numberformat) { get; set; } | Represents the custom display format of numbers and dates. |
| [OriginalItems](originalitems) { get; } | Get the original base items; |
| [PivotItems](pivotitems) { get; } | Gets the pivot items of the pivot field |
| [Position](position) { get; } | Represents the PivotField index in the PivotFields. |
| [Range](range) { get; } | Gets the group range of the pivot field |
| [ShowAllItems](showallitems) { get; set; } | Indicates whether all items in the PivotTable report are displayed, even if they don't contain summary data. show items with no data The default value is false. |
| [ShowCompact](showcompact) { get; set; } | Indicates whether display labels from the next field in the same column on the Pivot Table view |
| [ShowInOutlineForm](showinoutlineform) { get; set; } | Indicates whether layout this field in outline form on the Pivot Table view |
| [ShowSubtotalAtTop](showsubtotalattop) { get; set; } | when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |

## Methods

| Name | Description |
| --- | --- |
| [AddCalculatedItem](addcalculateditem)(string, string) | Add a calculated item to the pivot field. |
| [GetCalculatedFieldFormula](getcalculatedfieldformula)() | Get the formula string of the specified calculated field . |
| [GetPivotFilterByType](getpivotfilterbytype)(PivotFilterType) | Gets the pivot filter of the pivot field by type |
| [GetPivotFilters](getpivotfilters)() | Gets the pivot filters of the pivot field |
| [GetSubtotals](getsubtotals)(PivotFieldSubtotalType) | Gets whether the specified field shows that subtotals. |
| [HideDetail](hidedetail)(bool) | Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field. |
| [HideItem](hideitem)(int, bool) | Sets whether the specific PivotItem in a data field is hidden. |
| [HideItem](hideitem)(string, bool) | Sets whether the specific PivotItem in a data field is hidden. |
| [HideItemDetail](hideitemdetail)(int, bool) | Sets whether the specific PivotItem in a pivot field is hidden detail. |
| [InitPivotItems](initpivotitems)() | Init the pivot items of the pivot field |
| [IsHiddenItem](ishiddenitem)(int) | Indicates whether the specific PivotItem is hidden. |
| [IsHiddenItemDetail](ishiddenitemdetail)(int) | Indicates whether the specific PivotItem is hidden detail. |
| [SetSubtotals](setsubtotals)(PivotFieldSubtotalType, bool) | Sets whether the specified field shows that subtotals. |

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

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
