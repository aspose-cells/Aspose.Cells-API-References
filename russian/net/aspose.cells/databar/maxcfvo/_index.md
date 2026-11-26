---
title: "DataBar.MaxCfvo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataBar. Получает или задает объект максимального значения этой DataBar. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Min"
type: docs
url: /ru/net/aspose.cells/databar/maxcfvo/
---
## DataBar.MaxCfvo property

Получить или установить объект максимального значения этого DataBar. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Min.

```csharp
public ConditionalFormattingValue MaxCfvo { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMaxCfvoDemo
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

            // Добавить условное форматирование полос данных
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Добавить полосу данных
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[conditionIndex].DataBar;

            // Установить значение MaxCfvo
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            dataBar.MaxCfvo.Value = 50;

            // Сохраните книгу
            workbook.Save("DataBarMaxCfvoDemo.xlsx");
        }
    }
}
```

### См. также

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


