---
title: "Класс PivotConditionalFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotConditionalFormat. Представляет условное форматирование сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotconditionalformat/
---
## PivotConditionalFormat class

Представляет условное форматирование сводной таблицы.

```csharp
public class PivotConditionalFormat
```

## Свойства

| Имя | Описание |
| --- | --- |
| [FormatConditions](../../aspose.cells.pivot/pivotconditionalformat/formatconditions/) { get; } | Получить условия для условного форматирования сводной таблицы. |
| [PivotAreas](../../aspose.cells.pivot/pivotconditionalformat/pivotareas/) { get; } | Получает все области сводной таблицы. |
| [RuleType](../../aspose.cells.pivot/pivotconditionalformat/ruletype/) { get; set; } | Получить и установить тип правила для условного форматирования сводной таблицы. |
| [ScopeType](../../aspose.cells.pivot/pivotconditionalformat/scopetype/) { get; set; } | Получить и установить тип области для условного форматирования сводной таблицы. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddCellArea](../../aspose.cells.pivot/pivotconditionalformat/addcellarea/)(CellArea) | Добавляет область на основе представления сводной таблицы. |
| [AddFieldArea](../../aspose.cells.pivot/pivotconditionalformat/addfieldarea/#addfieldarea)(PivotFieldType, PivotField) | Добавляет область поля сводной таблицы. |
| [AddFieldArea](../../aspose.cells.pivot/pivotconditionalformat/addfieldarea/#addfieldarea_1)(PivotFieldType, string) | Добавляет область поля сводной таблицы. |
| [ApplyTo](../../aspose.cells.pivot/pivotconditionalformat/applyto/)(int, int, PivotConditionFormatScopeType) | Применяет условное форматирование к диапазону, который должен находиться в области данных. |
| [GetCellAreas](../../aspose.cells.pivot/pivotconditionalformat/getcellareas/)() | Получает все ячейковые области, к которым применяется это условное форматирование. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotClassPivotConditionalFormatDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Установить примерные данные
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";
            
            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;
            
            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;
            
            // Создать сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("=A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            
            // Добавить условное форматирование
            int formatIndex = pivot.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
            pfc.AddFieldArea(PivotFieldType.Data, pivot.DataFields[0]);
            
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = pfc.FormatConditions[conditionIndex];
            fc.Formula1 = "100";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;
            
            pivot.RefreshData();
            book.Save("PivotConditionalFormatDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


