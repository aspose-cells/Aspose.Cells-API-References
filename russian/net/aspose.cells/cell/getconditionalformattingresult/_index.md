---
title: "Cell.GetConditionalFormattingResult"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получить результат условного форматирования"
type: docs
url: /ru/net/aspose.cells/cell/getconditionalformattingresult/
---
## Cell.GetConditionalFormattingResult method

Получить результат условного форматирования.

```csharp
public ConditionalFormattingResult GetConditionalFormattingResult()
```

### Примечания

Возвращает null, если к этой ячейке не применено условное форматирование,

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetConditionalFormattingResultDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Добавить условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);
            
            // Установить условие и стиль
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fcc[conditionIndex].Style = style;

            // Получить результат условного форматирования для ячейки
            Cell cell = worksheet.Cells["A2"];
            ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
            
            // Вывести результат
            Console.WriteLine("Cell A2 meets condition: " + (result.ConditionalStyle != null));
            Console.WriteLine("Applied font color: " + result.ConditionalStyle.Font.Color);
        }
    }
}
```

### См. также

* class [ConditionalFormattingResult](../../conditionalformattingresult/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


