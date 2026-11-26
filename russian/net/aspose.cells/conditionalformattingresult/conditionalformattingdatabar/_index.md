---
title: "ConditionalFormattingResult.ConditionalFormattingDataBar"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConditionalFormattingResult. Возвращает объект DataBar"
type: docs
url: /ru/net/aspose.cells/conditionalformattingresult/conditionalformattingdatabar/
---
## ConditionalFormattingResult.ConditionalFormattingDataBar property

Получает объект DataBar.

```csharp
public DataBar ConditionalFormattingDataBar { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingResultPropertyConditionalFormattingDataBarDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные значения
            worksheet.Cells["A1"].PutValue(-6);
            worksheet.Cells["A2"].PutValue(-4);
            worksheet.Cells["A3"].PutValue(-2);
            worksheet.Cells["A4"].PutValue(0);
            worksheet.Cells["A5"].PutValue(2);
            worksheet.Cells["A6"].PutValue(4);
            worksheet.Cells["A7"].PutValue(6);

            // Добавить условное форматирование полос данных
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 6;
            area.EndColumn = 0;
            fcc.AddArea(area);

            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = fcc[conditionIndex];
            condition.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            condition.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            condition.DataBar.Color = System.Drawing.Color.Green;

            // Вычислите формулы и примените форматирование
            workbook.CalculateFormula();

            // Получите результат условного форматирования и продемонстрируйте свойства DataBar
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();
            
            Console.WriteLine("DataBar Min Value: " + formattingResult.ConditionalFormattingDataBar.MinCfvo.Value);
            Console.WriteLine("DataBar Max Value: " + formattingResult.ConditionalFormattingDataBar.MaxCfvo.Value);
            Console.WriteLine("DataBar Color: " + formattingResult.ConditionalFormattingDataBar.Color);
        }
    }
}
```

### См. также

* class [DataBar](../../databar/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


