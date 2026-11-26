---
title: "FormatCondition.AboveAverage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatCondition. Получить экземпляр условного форматирования AboveAverage. Правило экземпляра по умолчанию выделяет ячейки, значения которых выше среднего для всех значений в диапазоне. Действительно только для типа AboveAverage"
type: docs
url: /ru/net/aspose.cells/formatcondition/aboveaverage/
---
## FormatCondition.AboveAverage property

Получить экземпляр "AboveAverage" условного форматирования. Правило экземпляра по умолчанию выделяет ячейки, значения которых выше среднего для всех значений в диапазоне. Действительно только для type = AboveAverage.

```csharp
public AboveAverage AboveAverage { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyAboveAverageDemo
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
            worksheet.Cells["A5"].PutValue(50);

            // Добавить условное форматирование выше среднего
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 4, EndColumn = 0 });

            // Установить выделение значений выше среднего
            FormatCondition fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = true;
            fc.Style.BackgroundColor = Color.Yellow;

            // Добавить условное форматирование ниже среднего
            index = worksheet.ConditionalFormattings.Add();
            fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 1, EndRow = 4, EndColumn = 1 });

            // Установить выделение значений ниже среднего
            fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = false;
            fc.Style.BackgroundColor = Color.LightBlue;

            // Сохраните книгу
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### См. также

* class [AboveAverage](../../aboveaverage/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


