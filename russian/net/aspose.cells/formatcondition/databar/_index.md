---
title: "FormatCondition.DataBar"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatCondition. Получить экземпляр условного форматирования DataBar. Цвет экземпляра по умолчанию — синий. Действительно только для типа DataBar"
type: docs
url: /ru/net/aspose.cells/formatcondition/databar/
---
## FormatCondition.DataBar property

Получить экземпляр "DataBar" условного форматирования. Цвет экземпляра по умолчанию — синий. Действительно только для type = DataBar.

```csharp
public DataBar DataBar { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyDataBarDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Добавить условное форматирование полос данных
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Установить диапазон для условного форматирования
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Добавить условие полосы данных и задать свойства
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = fcs[conditionIndex];
            
            // Настроить свойства DataBar
            DataBar dataBar = condition.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            dataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            dataBar.Color = System.Drawing.Color.Green;

            // Сохраните книгу
            workbook.Save("DataBarExample.xlsx");
        }
    }
}
```

### См. также

* class [DataBar](../../databar/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


