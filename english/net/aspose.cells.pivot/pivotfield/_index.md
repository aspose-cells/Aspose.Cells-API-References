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
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield/) { get; set; } | Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields. |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotfield/basefieldindex/) { get; set; } | (**Obsolete.**) Represents the base field for a custom calculation when the ShowDataAs calculation is in use. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex/) { get; set; } | Represents the index in the source pivot fields. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotfield/baseitemindex/) { get; set; } | (**Obsolete.**) Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. |
| [BaseItemPosition](../../aspose.cells.pivot/pivotfield/baseitemposition/) { get; set; } | (**Obsolete.**) Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem/) { get; set; } | Represents the current selected page item of the page field to filter data. Only valid for page fields. |
| [DataDisplayFormat](../../aspose.cells.pivot/pivotfield/datadisplayformat/) { get; set; } | (**Obsolete.**) Represents how to display the values in a data field of the pivot report. |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname/) { get; set; } | Represents the display name of pivot field in the pivot table view. |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn/) { get; set; } | Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata/) { get; set; } | Indicates whether the specified field can be dragged to the values region. The default value is true. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide/) { get; set; } | Indicates whether the specified field can be dragged to the hide region. The default value is true. |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage/) { get; set; } | Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow/) { get; set; } | Indicates whether the specified field can be dragged to the row region. The default value is true. |
| [Function](../../aspose.cells.pivot/pivotfield/function/) { get; set; } | Represents the function used to summarize this PivotTable data field. |
| [GroupSettings](../../aspose.cells.pivot/pivotfield/groupsettings/) { get; } | Gets the group settings of the pivot field. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow/) { get; set; } | Indicates whether to insert a blank line after each item. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow/) { get; set; } | Indicates whether the specified PivotTable field is autoshown ascending. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort/) { get; set; } | Indicates whether the items of this pivot field is autosorted ascending. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow/) { get; set; } | Indicates whether the specified PivotTable field is automatically shown. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort/) { get; set; } | Indicates whether the items of this PivotTable field are automatically sorted. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals/) { get; set; } | Indicates whether the specified field shows automatic subtotals. Default is true. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield/) { get; } | Indicates whether the this pivot field is calculated field. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter/) { get; set; } | Indicates whether to include new items to the field in manual filter. The default value is false. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems/) { get; set; } | Indicates whether to insert page breaks after each item. The default value is false. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed/) { get; set; } | Indicates whether multiple items could be selected in the page field. The default value is false. |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels/) { get; set; } | Indicates whether to repeat labels of the field in the region. The default value is false. |
| [IsValueFields](../../aspose.cells.pivot/pivotfield/isvaluefields/) { get; } | (**Obsolete.**) Indicates whether this field represents values fields. |
| [IsValuesField](../../aspose.cells.pivot/pivotfield/isvaluesfield/) { get; } | Indicates whether this field represents values field. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount/) { get; } | Gets the count of the base items in this pivot field. |
| [Items](../../aspose.cells.pivot/pivotfield/items/) { get; } | Get all labels of pivot items in this field. |
| [Name](../../aspose.cells.pivot/pivotfield/name/) { get; set; } | Represents the name of PivotField. |
| [NonAutoSortDefault](../../aspose.cells.pivot/pivotfield/nonautosortdefault/) { get; set; } | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [Number](../../aspose.cells.pivot/pivotfield/number/) { get; set; } | Represents the built-in display format of numbers and dates. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat/) { get; set; } | Represents the custom display format of numbers and dates. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems/) { get; } | Get the original base items; |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems/) { get; } | Gets the pivot items of the pivot field |
| [Position](../../aspose.cells.pivot/pivotfield/position/) { get; } | Represents the index of `PivotField` in the region. |
| [RegionType](../../aspose.cells.pivot/pivotfield/regiontype/) { get; } | Specifies the region of the PivotTable that this field is displayed. |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems/) { get; set; } | Indicates whether to display all items in the PivotTable view, even if they don't contain summary data. The default value is false. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact/) { get; set; } | Indicates whether to display labels of the next field in the same column on the Pivot Table view |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform/) { get; set; } | Indicates whether to layout this field in outline form on the Pivot Table view. |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop/) { get; set; } | Indicates whether to display subtotals at the top or bottom of items when ShowInOutlineForm is true, then |
| [ShowValuesSetting](../../aspose.cells.pivot/pivotfield/showvaluessetting/) { get; } | Gets the settings of showing values as when the ShowDataAs calculation is in use. |
| [SortSetting](../../aspose.cells.pivot/pivotfield/sortsetting/) { get; } | Gets all settings of auto sorting |

## Methods

| Name | Description |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem/)(string, string) | Add a calculated formula item to the pivot field. |
| [ClearFilter](../../aspose.cells.pivot/pivotfield/clearfilter/)() | Clears filter setting on this pivot field. |
| [FilterByDate](../../aspose.cells.pivot/pivotfield/filterbydate/)(PivotFilterType, DateTime, DateTime) | Filters by date values of row or column pivot field. |
| [FilterByLabel](../../aspose.cells.pivot/pivotfield/filterbylabel/)(PivotFilterType, string, string) | Filters by captions of row or column pivot field. |
| [FilterByValue](../../aspose.cells.pivot/pivotfield/filterbyvalue/)(int, PivotFilterType, double, double) | Filters by values of data pivot field. |
| [FilterTop10](../../aspose.cells.pivot/pivotfield/filtertop10/)(int, PivotFilterType, bool, int) | Filters by values of data pivot field. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula/)() | (**Obsolete.**) Get the formula string of the specified calculated field . |
| [GetFilters](../../aspose.cells.pivot/pivotfield/getfilters/)() | Gets all pivot filters applied for this pivot field. |
| [GetFormula](../../aspose.cells.pivot/pivotfield/getformula/)() | Gets the formula of the calculated field . Only works for calculated field. |
| [GetMaxValue](../../aspose.cells.pivot/pivotfield/getmaxvalue/)() | Gets the max value of this field. |
| [GetMinValue](../../aspose.cells.pivot/pivotfield/getminvalue/)() | Gets the max value of this field. |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype/)(PivotFilterType) | Gets the pivot filter of the pivot field by type |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters/)() | (**Obsolete.**) Gets the pivot filters of the pivot field |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals/)(PivotFieldSubtotalType) | Indicates whether to show specified subtotal for this pivot field. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby)(CustomPiovtFieldGroupItem[], bool) | Custom group the field. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_6)(double, bool) | Automatically group the field with internal |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_5)(PivotGroupByType[], double, bool) | Automatically group the field with internal |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_3)(double, double, double, bool) | Group the file by number. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_4)(DateTime, DateTime, PivotGroupByType[], double, bool) | Group the file by the date group types. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_1)(bool, double, bool, double, double, bool) | Group the file by number. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_2)(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) | Group the file by the date group types. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail/)(bool) | Sets whether the detail of all PivotItems in a pivot field are hidden. That is collapse/expand this field. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem/#hideitem)(int, bool) | Sets whether the specific PivotItem in a data field is hidden. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem/#hideitem_1)(string, bool) | Sets whether the specific PivotItem in a data field is hidden. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail/)(int, bool) | Sets whether the specific PivotItem in a pivot field is hidden detail. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems/)() | Init the pivot items of the pivot field |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem/)(int) | Gets whether the specific PivotItem is hidden. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail/)(int) | Gets whether to hide the detail of the specific PivotItem.. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals/)(PivotFieldSubtotalType, bool) | Sets how to subtotal the specified field. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/)(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) | Shows values of data field as different display format when the ShowDataAs calculation is in use. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby)(SortOrder, int) | Sorts this pivot field. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_1)(SortOrder, int, PivotLineType, string) | Sorts this pivot field. |
| [Ungroup](../../aspose.cells.pivot/pivotfield/ungroup/)() | Ungroup the pivot field. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldDemo
    {
        public static void PivotFieldExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Add some data to the worksheet
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

            // Add a pivot table to the worksheet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "year");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "amount");

            // Set pivot table style
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Access the row field
            PivotField rowField = pivotTable.RowFields[0];

            // Set properties of the PivotField
            rowField.DisplayName = "Custom Display Name";
            rowField.IsAutoSubtotals = false;
            rowField.DragToColumn = true;
            rowField.DragToHide = true;
            rowField.DragToRow = true;
            rowField.DragToPage = true;
            rowField.DragToData = true;
            rowField.IsMultipleItemSelectionAllowed = true;
            rowField.IsRepeatItemLabels = true;
            rowField.IsIncludeNewItemsInFilter = true;
            rowField.IsInsertPageBreaksBetweenItems = true;
            rowField.ShowAllItems = true;
            rowField.NonAutoSortDefault = true;
            rowField.IsAutoSort = true;
            rowField.IsAscendSort = true;
            rowField.AutoSortField = -1;
            rowField.IsAutoShow = true;
            rowField.IsAscendShow = true;
            rowField.AutoShowCount = 5;
            rowField.AutoShowField = -1;
            rowField.Function = ConsolidationFunction.Sum;
            rowField.DataDisplayFormat = PivotFieldDataDisplayFormat.PercentageOfTotal;
            rowField.BaseFieldIndex = 0;
            rowField.BaseItemPosition = PivotItemPosition.Next;
            rowField.BaseItemIndex = 0;
            rowField.CurrentPageItem = 1;
            rowField.Number = 0;
            rowField.InsertBlankRow = true;
            rowField.ShowSubtotalAtTop = true;
            rowField.ShowInOutlineForm = true;
            rowField.NumberFormat = "0.00";
            rowField.ShowCompact = true;

            // Refresh and calculate the pivot table data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Save the workbook
            workbook.Save("PivotFieldExample.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


