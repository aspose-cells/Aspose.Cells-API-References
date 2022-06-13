---
title: PivotFormatCondition
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет условие формата сводной таблицы в коллекции PivotFormatCondition.
type: docs
weight: 4610
url: /ru/net/aspose.cells.pivot/pivotformatcondition/
---
## PivotFormatCondition class

Представляет условие формата сводной таблицы в коллекции PivotFormatCondition.

```csharp
public class PivotFormatCondition
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [FormatConditions](../../aspose.cells.pivot/pivotformatcondition/formatconditions) { get; } | Получить formatconditions для формата условия сводной таблицы. |
| [RuleType](../../aspose.cells.pivot/pivotformatcondition/ruletype) { get; set; } | Получить и установить тип правила для формата условия сводной таблицы. |
| [ScopeType](../../aspose.cells.pivot/pivotformatcondition/scopetype) { get; set; } | Получить и установить тип области для формата условий сводной таблицы. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddColumnAreaCondition](../../aspose.cells.pivot/pivotformatcondition/addcolumnareacondition#addcolumnareacondition)(PivotField) | Добавляет ограничение условного формата сводной таблицы в поля столбца. |
| [AddColumnAreaCondition](../../aspose.cells.pivot/pivotformatcondition/addcolumnareacondition#addcolumnareacondition_1)(string) | Добавляет ограничение условного формата сводной таблицы в поля столбца. |
| [AddDataAreaCondition](../../aspose.cells.pivot/pivotformatcondition/adddataareacondition#adddataareacondition)(PivotField) | Добавляет ограничение условного формата сводной таблицы в поля данных. |
| [AddDataAreaCondition](../../aspose.cells.pivot/pivotformatcondition/adddataareacondition#adddataareacondition_1)(string) | Добавляет ограничение условного формата сводной таблицы в поля данных. |
| [AddRowAreaCondition](../../aspose.cells.pivot/pivotformatcondition/addrowareacondition#addrowareacondition)(PivotField) | Добавляет ограничение условного формата сводной таблицы в поля строки. |
| [AddRowAreaCondition](../../aspose.cells.pivot/pivotformatcondition/addrowareacondition#addrowareacondition_1)(string) | Добавляет ограничение условного формата сводной таблицы в поля строки. |
| [SetConditionalAreas](../../aspose.cells.pivot/pivotformatcondition/setconditionalareas)() | Задает условные области объекта PivotFormatCondition. |

### Примеры

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

  //Добавить PivotFormatCondition
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

  //делай свое дело

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

'Add PivotFormatCondition
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

### Смотрите также

* пространство имен [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
