---
title: Class PivotFieldTop10AutoShowSettings
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotFieldTop10AutoShowSettings class. Represents the Top 10 AutoShow settings for a pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfieldtop10autoshowsettings/
---
## PivotFieldTop10AutoShowSettings class

Represents the Top 10 AutoShow settings for a pivot field.

```csharp
public class PivotFieldTop10AutoShowSettings
```

## Properties

| Name | Description |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/autoshowcount/) { get; set; } | Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/isautoshow/) { get; set; } | Indicates whether an "Top 10 AutoShow" filter is applied to this field. |
| [IsTop](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/istop/) { get; set; } | Indicates whether the specified PivotTable field is autoshown ascending. |
| [RankBy](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/rankby/) { get; set; } | Specifies the index of data field for AutoShow ranking. Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields. |

### Remarks

In xls : Implementing top 10 filters in Xls through Top 10 AutoShow In ooxml files: The underlying ooxml file format supports Top10 AutoShow, but Excel 2007 and later user interface only provides access via Top10 filter. If XLS compatibility is not required, it is recommended to use Top10 filter instead.

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

PivotTable pivot = pivots.Add("=Sheet1!A1:C9", "A12");

pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
           
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
           
 //Change PivotField's attributes
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

//Show top 2 items by row field label.
rowField.Top10AutoShow(true, true, 2, -1);

PivotFieldTop10AutoShowSettings sortSetting = rowField.Top10AutoShowSettings;
Console.WriteLine(sortSetting.IsAutoShow);

 pivot.CalculateData();

book.Save("out.xlsx");

[Visual Basic]

Dim book As New Workbook()
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

Dim pivot As PivotTable = pivots.Add("=Sheet1!A1:C9", "A12")
 
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
pivot.AddFieldToArea(PivotFieldType.Column, "year")
pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'Show top 2 items by row field label.
rowField.Top10AutoShow(True, True, 2, -1)

Dim sortSetting As PivotFieldTop10AutoShowSettings = rowField.Top10AutoShowSettings
Console.WriteLine(sortSetting.IsAutoShow)

pivot.CalculateData()

book.Save("out.xlsx")
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


