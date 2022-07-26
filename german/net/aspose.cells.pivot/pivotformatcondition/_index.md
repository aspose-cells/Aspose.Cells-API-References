---
title: PivotFormatCondition
second_title: Aspose.Cells für .NET-API-Referenz
description: Stellt eine PivotTable-Formatbedingung in der PivotFormatCondition-Auflistung dar.
type: docs
weight: 4610
url: /de/net/aspose.cells.pivot/pivotformatcondition/
---
## PivotFormatCondition class

Stellt eine PivotTable-Formatbedingung in der PivotFormatCondition-Auflistung dar.

```csharp
public class PivotFormatCondition
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FormatConditions](../../aspose.cells.pivot/pivotformatcondition/formatconditions) { get; } | Formatbedingungen für das Bedingungsformat der Pivot-Tabelle abrufen . |
| [RuleType](../../aspose.cells.pivot/pivotformatcondition/ruletype) { get; set; } | Abrufen und Festlegen des Regeltyps für das Bedingungsformat der Pivot-Tabelle . |
| [ScopeType](../../aspose.cells.pivot/pivotformatcondition/scopetype) { get; set; } | Abrufen und Festlegen des Bereichstyps für das Bedingungsformat der Pivot-Tabelle . |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddColumnAreaCondition](../../aspose.cells.pivot/pivotformatcondition/addcolumnareacondition#addcolumnareacondition)(PivotField) | Fügt das bedingte PivotTable-Formatlimit in den Spaltenfeldern hinzu. |
| [AddColumnAreaCondition](../../aspose.cells.pivot/pivotformatcondition/addcolumnareacondition#addcolumnareacondition_1)(string) | Fügt das bedingte PivotTable-Formatlimit in den Spaltenfeldern hinzu. |
| [AddDataAreaCondition](../../aspose.cells.pivot/pivotformatcondition/adddataareacondition#adddataareacondition)(PivotField) | Fügt das bedingte PivotTable-Formatlimit in den Datenfeldern hinzu. |
| [AddDataAreaCondition](../../aspose.cells.pivot/pivotformatcondition/adddataareacondition#adddataareacondition_1)(string) | Fügt das bedingte PivotTable-Formatlimit in den Datenfeldern hinzu. |
| [AddRowAreaCondition](../../aspose.cells.pivot/pivotformatcondition/addrowareacondition#addrowareacondition)(PivotField) | Fügt das bedingte PivotTable-Formatlimit in den Zeilenfeldern hinzu. |
| [AddRowAreaCondition](../../aspose.cells.pivot/pivotformatcondition/addrowareacondition#addrowareacondition_1)(string) | Fügt das bedingte PivotTable-Formatlimit in den Zeilenfeldern hinzu. |
| [SetConditionalAreas](../../aspose.cells.pivot/pivotformatcondition/setconditionalareas)() | Legt bedingte Bereiche des PivotFormatCondition-Objekts fest. |

### Beispiele

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

//PivotFormatCondition hinzufügen
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

// Mach dein Geschäft

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

'Fügen Sie PivotFormatCondition hinzu
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

### Siehe auch

* namensraum [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
