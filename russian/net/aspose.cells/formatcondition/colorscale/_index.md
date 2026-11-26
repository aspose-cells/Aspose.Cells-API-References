---
title: "FormatCondition.ColorScale"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatCondition. Получить экземпляр ColorScale условного форматирования. Экземпляр по умолчанию — зеленый‑желтый‑красный 3ColorScale. Доступно только для типа ColorScale."
type: docs
url: /ru/net/aspose.cells/formatcondition/colorscale/
---
## FormatCondition.ColorScale property

Получить экземпляр "ColorScale" условного форматирования. Экземпляр по умолчанию представляет собой "green-yellow-red" 3ColorScale. Действительно только для type = ColorScale.

```csharp
public ColorScale ColorScale { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyColorScaleDemo
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

            // Добавить условное форматирование цветовой шкалы
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Установить диапазон для условного форматирования
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Установить свойства цветовой шкалы
            fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[0];
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Green;

            // Сохраните книгу
            workbook.Save("ColorScaleExample.xlsx");
        }
    }
}
```

### См. также

* class [ColorScale](../../colorscale/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


