---
title: PivotFilter
second_title: Aspose.Cells för .NET API-referens
description: Representerar ett PivotFilter i PivotFilter Collection.
type: docs
weight: 4580
url: /sv/net/aspose.cells.pivot/pivotfilter/
---
## PivotFilter class

Representerar ett PivotFilter i PivotFilter Collection.

```csharp
public class PivotFilter
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AutoFilter](../../aspose.cells.pivot/pivotfilter/autofilter) { get; } | Hämtar autofiltret för pivotfiltret. |
| [EvaluationOrder](../../aspose.cells.pivot/pivotfilter/evaluationorder) { get; set; } | Hämtar utvärderingsordningen för pivotfiltret. |
| [FieldIndex](../../aspose.cells.pivot/pivotfilter/fieldindex) { get; } | Hämtar fältindexet för pivotfiltret. |
| [FilterType](../../aspose.cells.pivot/pivotfilter/filtertype) { get; } | Hämtar autofiltertypen för pivotfiltret. |
| [MeasureFldIndex](../../aspose.cells.pivot/pivotfilter/measurefldindex) { get; set; } | Hämtar mätfältsindex för pivotfiltret. |
| [MemberPropertyFieldIndex](../../aspose.cells.pivot/pivotfilter/memberpropertyfieldindex) { get; set; } | Hämtar medlemsegenskapsfältindex för pivotfiltret. |
| [Name](../../aspose.cells.pivot/pivotfilter/name) { get; set; } | Hämtar namnet på pivotfiltret. |
| [Value1](../../aspose.cells.pivot/pivotfilter/value1) { get; set; } | Hämtar strängvärdet1 för etikettens pivotfilter. |
| [Value2](../../aspose.cells.pivot/pivotfilter/value2) { get; set; } | Hämtar strängvärdet2 för etikettens pivotfilter. |

### Exempel

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

//Lägg till PivotFilter
int index = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[index];
filter.AutoFilter.FilterTop10(0, false, false, 2);

pivot.RefreshData();
pivot.CalculateData();

//gör dina affärer

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

'Lägg till PivotFilter
Dim filterIndex As Int32 = pivot.PivotFilters.Add(0, PivotFilterType.Count)
Dim filter As PivotFilter = pivot.PivotFilters(filterIndex)
filter.AutoFilter.FilterTop10(0, False, False, 2)

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Se även

* namnutrymme [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->