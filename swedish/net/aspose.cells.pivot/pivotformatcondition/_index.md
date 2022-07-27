---
title: PivotFormatCondition
second_title: Aspose.Cells för .NET API-referens
description: Representerar ett pivottabellformatvillkor i PivotFormatCondition Collection.
type: docs
weight: 4610
url: /sv/net/aspose.cells.pivot/pivotformatcondition/
---
## PivotFormatCondition class

Representerar ett pivottabellformatvillkor i PivotFormatCondition Collection.

```csharp
public class PivotFormatCondition
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [FormatConditions](../../aspose.cells.pivot/pivotformatcondition/formatconditions) { get; } | Hämta formatvillkor för pivottabellens villkorsformat . |
| [RuleType](../../aspose.cells.pivot/pivotformatcondition/ruletype) { get; set; } | Hämta och ställ in regeltyp för pivottabellens villkorsformat . |
| [ScopeType](../../aspose.cells.pivot/pivotformatcondition/scopetype) { get; set; } | Hämta och ställ in omfattningstyp för pivottabellens villkorsformat . |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [AddColumnAreaCondition](../../aspose.cells.pivot/pivotformatcondition/addcolumnareacondition#addcolumnareacondition)(PivotField) | Lägger till PivotTables villkorliga formatgräns i kolumnfälten. |
| [AddColumnAreaCondition](../../aspose.cells.pivot/pivotformatcondition/addcolumnareacondition#addcolumnareacondition_1)(string) | Lägger till PivotTables villkorliga formatgräns i kolumnfälten. |
| [AddDataAreaCondition](../../aspose.cells.pivot/pivotformatcondition/adddataareacondition#adddataareacondition)(PivotField) | Lägger till PivotTables villkorliga formatgräns i datafälten. |
| [AddDataAreaCondition](../../aspose.cells.pivot/pivotformatcondition/adddataareacondition#adddataareacondition_1)(string) | Lägger till PivotTables villkorliga formatgräns i datafälten. |
| [AddRowAreaCondition](../../aspose.cells.pivot/pivotformatcondition/addrowareacondition#addrowareacondition)(PivotField) | Lägger till PivotTables villkorliga formatgräns i radfälten. |
| [AddRowAreaCondition](../../aspose.cells.pivot/pivotformatcondition/addrowareacondition#addrowareacondition_1)(string) | Lägger till PivotTables villkorliga formatgräns i radfälten. |
| [SetConditionalAreas](../../aspose.cells.pivot/pivotformatcondition/setconditionalareas)() | Ställer in villkorliga områden för PivotFormatCondition-objektet. |

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

//Lägg till PivotFormatCondition
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;

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

'Lägg till PivotFormatCondition
Dim formatIndex As Int32 = pivot.PivotFormatConditions.Add()
Dim pfc As PivotFormatCondition = pivot.PivotFormatConditions(formatIndex)
Dim fcc As FormatConditionCollection = pfc.FormatConditions
fcc.AddArea(pivot.DataBodyRange)
Dim idx As Int32 = fcc.AddCondition(FormatConditionType.CellValue)
Dim fc As FormatCondition = fcc(idx)
fc.Formula1 = "100"
fc.Operator = OperatorType.GreaterOrEqual
fc.Style.BackgroundColor = Color.Red

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Se även

* namnutrymme [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
