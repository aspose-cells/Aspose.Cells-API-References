---
title: PivotField
second_title: Aspose.Cells for .NET API 参考
description: 表示数据透视表中的一个字段
type: docs
weight: 4530
url: /zh/net/aspose.cells.pivot/pivotfield/
---
## PivotField class

表示数据透视表中的一个字段。

```csharp
public class PivotField
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount) { get; set; } | 表示在指定数据透视表字段中自动显示的顶部或底部项目数 。 |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield) { get; set; } | 表示自动显示字段索引。 -1 表示 PivotField 本身。 应该是数据字段的索引。 |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield) { get; set; } | 表示自动排序字段索引。 -1 表示 PivotField 本身，其他表示数据字段的位置。 |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotfield/basefieldindex) { get; set; } | 表示自定义计算的基本字段。 |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex) { get; set; } | 表示基础 PivotFields 中的 PivotField 索引。 |
| [BaseItemIndex](../../aspose.cells.pivot/pivotfield/baseitemindex) { get; set; } | 表示自定义计算的基本字段中的项目。 仅对数据字段有效。 |
| [BaseItemPosition](../../aspose.cells.pivot/pivotfield/baseitemposition) { get; set; } | 表示自定义计算的基本字段中的项目。 仅对数据字段有效。 因为PivotItemPosition.Custom是只读的，如果需要设置PivotItemPosition.Custom， 请设置PivotField.BaseItemIndex属性。 |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem) { get; set; } | 表示为页面字段显示的当前页面项目（仅对页面字段有效）。 |
| [DataDisplayFormat](../../aspose.cells.pivot/pivotfield/datadisplayformat) { get; set; } | 表示如何显示数据字段中包含的值。 |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname) { get; set; } | 表示 PivotField 显示名称。 |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn) { get; set; } | 表示是否可以将指定字段拖到列位置。 默认值为true。 |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata) { get; set; } | 表示是否可以将指定字段拖到数据位置。 默认值为true。 |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide) { get; set; } | 表示是否可以将指定字段拖到隐藏位置。 默认值为true。 |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage) { get; set; } | 表示是否可以将指定字段拖到页面位置。 默认值为true。 |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow) { get; set; } | 表示是否可以将指定字段拖到行位置。 默认值为true。 |
| [Function](../../aspose.cells.pivot/pivotfield/function) { get; set; } | 表示用于汇总数据透视表数据字段的函数。 |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow) { get; set; } | 表示是否在每一项后插入空行。 |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow) { get; set; } | 指示指定的数据透视表字段是否自动升序显示。 |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort) { get; set; } | 指示指定的数据透视表字段是否自动升序排序。 |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow) { get; set; } | 表示指定的数据透视表字段是否自动显示，仅对excel 2003有效。 |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort) { get; set; } | 表示指定的数据透视表字段是否自动排序。 |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals) { get; set; } | 指示指定字段是否显示自动小计。默认为真。 |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield) { get; } | 表示指定的数据透视表字段是否为计算字段。 |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter) { get; set; } | 表示该字段是否可以包含手动过滤器中的新项目 默认值为false。 |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems) { get; set; } | 表示字段是否可以在item之间插入分页符 在每个item之后插入分页符 默认值为false。 |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed) { get; set; } | 表示该字段是否可以有多个项目 在页面中选择字段 默认值为false。 |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels) { get; set; } | 表示该字段是否可以重复项labels 默认值为false。 |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount) { get; } | 获取此数据透视字段的基本项目数。 |
| [Items](../../aspose.cells.pivot/pivotfield/items) { get; } | 获取所有基础物品； |
| [Name](../../aspose.cells.pivot/pivotfield/name) { get; } | 表示数据透视字段名称。 |
| [Number](../../aspose.cells.pivot/pivotfield/number) { get; set; } | 表示数字和日期的内置显示格式。 |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat) { get; set; } | 表示数字和日期的自定义显示格式。 |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems) { get; } | 获取原始基础物品； |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems) { get; } | 获取枢轴字段的枢轴项 |
| [Position](../../aspose.cells.pivot/pivotfield/position) { get; } | 表示 PivotFields 中的 PivotField 索引。 |
| [Range](../../aspose.cells.pivot/pivotfield/range) { get; } | 获取枢轴字段的组范围 |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems) { get; set; } | 表示是否显示数据透视表中的所有项目， 即使它们不包含汇总数据。 显示没有数据的项目 默认值为false。 |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact) { get; set; } | 表示是否在数据透视表视图的同一列中显示来自下一个字段的标签 |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform) { get; set; } | 指示是否在数据透视表视图上以大纲形式布局此字段 |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop) { get; set; } | 当 ShowInOutlineForm 为真时，然后在项目列表的顶部而不是底部显示小计 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem)(string, string) | 将计算项添加到数据透视字段。 |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula)() | 获取指定计算字段的公式字符串. |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype)(PivotFilterType) | 通过type 获取pivot字段的pivot过滤器 |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters)() | 获取枢轴字段 的枢轴过滤器 |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals)(PivotFieldSubtotalType) | 获取指定字段是否显示小计。 |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail)(bool) | 设置pivot字段中的PivotItems是否隐藏细节。即折叠/展开该字段。 |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem)(int, bool) | 设置数据字段中的特定 PivotItem 是否隐藏。 |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem_1)(string, bool) | 设置数据字段中的特定 PivotItem 是否隐藏。 |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail)(int, bool) | 设置数据透视字段中的特定 PivotItem 是否隐藏细节。 |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems)() | 初始化pivot字段的pivot项 |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem)(int) | 指示特定的 PivotItem 是否隐藏。 |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail)(int) | 指示特定 PivotItem 是否为隐藏细节。 |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals)(PivotFieldSubtotalType, bool) | 设置指定字段是否显示小计。 |

### 例子

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

//改变PivotField的属性
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

pivot.RefreshData();
pivot.CalculateData();

//做你的事

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

### 也可以看看

* 命名空间 [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
