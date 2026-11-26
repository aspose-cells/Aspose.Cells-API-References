---
title: "Worksheet.ConditionalFormattings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Возвращает ConditionalFormattings в листе"
type: docs
url: /ru/net/aspose.cells/worksheet/conditionalformattings/
---
## Worksheet.ConditionalFormattings property

Получает ConditionalFormattings в рабочем листе.

```csharp
public ConditionalFormattingCollection ConditionalFormattings { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyConditionalFormattingsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Создайте условное форматирование
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            
            // Установить диапазон
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Добавить условие
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "15", null);
            FormatCondition fc = fcc[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Red;

            // Сохраните книгу
            workbook.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### См. также

* class [ConditionalFormattingCollection](../../conditionalformattingcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


