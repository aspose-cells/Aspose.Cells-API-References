---
title: Class PivotFilter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotFilter class. Represents a PivotFilter in PivotFilter Collection
type: docs
url: /net/aspose.cells.pivot/pivotfilter/
---
## PivotFilter class

Represents a PivotFilter in PivotFilter Collection.

```csharp
public class PivotFilter
```

## Properties

| Name | Description |
| --- | --- |
| [AutoFilter](../../aspose.cells.pivot/pivotfilter/autofilter/) { get; } | (**Obsolete.**) Gets the autofilter of the pivot filter. |
| [EvaluationOrder](../../aspose.cells.pivot/pivotfilter/evaluationorder/) { get; set; } | Gets the Evaluation Order of the pivot filter. |
| [FieldIndex](../../aspose.cells.pivot/pivotfilter/fieldindex/) { get; } | Gets the index of source field which this pivot filter is applied to. |
| [FilterCategory](../../aspose.cells.pivot/pivotfilter/filtercategory/) { get; } | Gets the category of this filter. |
| [FilterType](../../aspose.cells.pivot/pivotfilter/filtertype/) { get; } | Gets the filter type of the pivot filter. |
| [MeasureCubeFieldIndex](../../aspose.cells.pivot/pivotfilter/measurecubefieldindex/) { get; } | Specifies the index of the measure cube field. this property is used only by filters in OLAP pivots and specifies on which measure a value filter should apply. |
| [MeasureFldIndex](../../aspose.cells.pivot/pivotfilter/measurefldindex/) { get; set; } | (**Obsolete.**) Gets the measure field index of the pivot filter. |
| [MemberPropertyFieldIndex](../../aspose.cells.pivot/pivotfilter/memberpropertyfieldindex/) { get; set; } | Gets the member property field index of the pivot filter. |
| [Name](../../aspose.cells.pivot/pivotfilter/name/) { get; set; } | Gets the name of the pivot filter. |
| [UseWholeDay](../../aspose.cells.pivot/pivotfilter/usewholeday/) { get; set; } | Indicates whether to use whole days in its date filtering criteria. |
| [Value1](../../aspose.cells.pivot/pivotfilter/value1/) { get; set; } | Gets the string value1 of the label pivot filter. |
| [Value2](../../aspose.cells.pivot/pivotfilter/value2/) { get; set; } | Gets the string value2 of the label pivot filter. |
| [ValueFieldIndex](../../aspose.cells.pivot/pivotfilter/valuefieldindex/) { get; set; } | Gets the index of value field in the value region. |

## Methods

| Name | Description |
| --- | --- |
| [GetDateTimeValues](../../aspose.cells.pivot/pivotfilter/getdatetimevalues/)() | Gets values of the number filter. |
| [GetLabels](../../aspose.cells.pivot/pivotfilter/getlabels/)() | Gets labels of the caption filter. |
| [GetNumberValues](../../aspose.cells.pivot/pivotfilter/getnumbervalues/)() | Gets values of the number filter. |
| [GetTop10Value](../../aspose.cells.pivot/pivotfilter/gettop10value/)() | Gets top 10 setting of the filter. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterDemo
    {
        public static void PivotFilterExample()
        {
            // Create a new workbook
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Populate the worksheet with sample data
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
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Set pivot table style
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Add a pivot filter
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Set additional properties for the pivot filter
            filter.Value1 = "SampleValue1";
            filter.Value2 = "SampleValue2";
            filter.MeasureFldIndex = 1;
            filter.MemberPropertyFieldIndex = 2;
            filter.Name = "SampleFilter";
            filter.EvaluationOrder = 1;

            // Refresh and calculate the pivot table data
            pivot.RefreshData();
            pivot.CalculateData();

            // Save the workbook
            book.Save("PivotFilterExample.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


