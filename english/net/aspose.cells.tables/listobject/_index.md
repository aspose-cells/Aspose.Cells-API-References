---
title: Class ListObject
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Tables.ListObject class. Represents a table in a worksheet
type: docs
url: /net/aspose.cells.tables/listobject/
---
## ListObject class

Represents a table in a worksheet.

```csharp
public class ListObject
```

## Properties

| Name | Description |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription/) { get; set; } | Gets and sets the alternative description. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext/) { get; set; } | Gets and sets the alternative text. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter/) { get; } | Gets auto filter of this table. |
| [Comment](../../aspose.cells.tables/listobject/comment/) { get; set; } | Gets and sets the comment of the table. |
| [DataRange](../../aspose.cells.tables/listobject/datarange/) { get; } | Gets the data range of the Table. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype/) { get; } | Gets the data source type of the table. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname/) { get; set; } | Gets and sets the display name of the table. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn/) { get; } | Gets the end column of the range. |
| [EndRow](../../aspose.cells.tables/listobject/endrow/) { get; } | Gets the end row of the range. |
| [HasAutoFilter](../../aspose.cells.tables/listobject/hasautofilter/) { get; set; } | Indicates whether auto filter is applied to this table. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns/) { get; } | Gets the [`ListColumn`](../listcolumn/) list of this table. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable/) { get; } | Gets the linked QueryTable. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow/) { get; set; } | Gets and sets whether this Table shows header row. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes/) { get; set; } | Indicates whether column stripe formatting is applied to. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn/) { get; set; } | Indicates whether the first column in the table is the style applied to. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn/) { get; set; } | Indicates whether the last column in the table is the style applied to. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes/) { get; set; } | Indicates whether row stripe formatting is applied to. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals/) { get; set; } | Gets and sets whether this TAble shows total row. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn/) { get; } | Gets the start column of the range. |
| [StartRow](../../aspose.cells.tables/listobject/startrow/) { get; } | Gets the start row of the range. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename/) { get; set; } | Gets and sets the table style name. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype/) { get; set; } | Gets and the built-in table style. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap/) { get; } | Gets an [`XmlMap`](./xmlmap/) used for this list. |

## Methods

| Name | Description |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange/)() | Apply the table style to the range. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange)() | Convert the table to range. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange_1)(TableToRangeOptions) | Convert the table to range. |
| [Filter](../../aspose.cells.tables/listobject/filter/)() | (**Obsolete.**) Filter the table. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula)(int, int, string) | Put the formula to the cell in the table. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula_1)(int, int, string, bool) | Put the formula to the cell in the table. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue)(int, int, object) | Put the value to the cell. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue_1)(int, int, object, bool) | Put the value to the cell. |
| [RemoveAutoFilter](../../aspose.cells.tables/listobject/removeautofilter/)() | Removes auto filter which is applied to this table. |
| [Resize](../../aspose.cells.tables/listobject/resize/)(int, int, int, int, bool) | Resize the range of the list object. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname/)() | Updates all list columns' name to cells in the table. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectDemo
    {
        public static void ListObjectExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Populate the worksheet with some data
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Add a ListObject (table) to the worksheet
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Set some properties of the ListObject
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;
            table.DisplayName = "SampleTable";
            table.Comment = "This is a sample table.";
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.ShowTableStyleRowStripes = true;
            table.ShowTableStyleColumnStripes = true;
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Save the workbook
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


