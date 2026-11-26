---
title: "PivotConditionalFormat.ScopeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotConditionalFormat. Получайте и задавайте тип области для условного форматирования сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotconditionalformat/scopetype/
---
## PivotConditionalFormat.ScopeType property

Получить и установить тип области для условного форматирования сводной таблицы.

```csharp
public PivotConditionFormatScopeType ScopeType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatPropertyScopeTypeDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу со сводной таблицей
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Пример данных для сводной таблицы
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(300);

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Добавьте условное форматирование в сводную таблицу
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
            pcf.ScopeType = PivotConditionFormatScopeType.Data;

            // Добавить условие форматирования
            FormatConditionCollection fcs = pcf.FormatConditions;
            CellArea area = new CellArea();
            area.StartRow = 4;
            area.EndRow = 6;
            area.StartColumn = 5;
            area.EndColumn = 5;
            int[] conditionIndex = fcs.Add(area, FormatConditionType.CellValue, OperatorType.Between, "100", "200");
            
            // Установите стиль формата
            FormatCondition fc = fcs[conditionIndex[0]];
            fc.Style.BackgroundColor = Color.Yellow;

            // Сохраните книгу
            wb.Save("PivotConditionalFormatScopeTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


