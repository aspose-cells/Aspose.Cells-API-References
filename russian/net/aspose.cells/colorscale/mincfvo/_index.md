---
title: "ColorScale.MinCfvo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ColorScale. Получает или задает объект минимального значения этой шкалы цветов. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Max"
type: docs
url: /ru/net/aspose.cells/colorscale/mincfvo/
---
## ColorScale.MinCfvo property

Получить или установить объект минимального значения этого ColorScale. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Max.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMinCfvoDemo
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

            // Создать условное форматирование цветовой шкалы
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Добавить цветовую шкалу
            int csIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            ColorScale cs = fcc[csIndex].ColorScale;

            // Установить свойства MinCfvo
            cs.MinCfvo.Type = FormatConditionValueType.Min;
            cs.MinCfvo.Value = "0";
            cs.MinColor = System.Drawing.Color.Red;

            // Установить свойства MidCfvo
            cs.MidCfvo.Type = FormatConditionValueType.Percentile;
            cs.MidCfvo.Value = "50";
            cs.MidColor = System.Drawing.Color.Yellow;

            // Установить свойства MaxCfvo
            cs.MaxCfvo.Type = FormatConditionValueType.Max;
            cs.MaxCfvo.Value = "0";
            cs.MaxColor = System.Drawing.Color.Green;

            // Сохраните книгу
            workbook.Save("ColorScaleMinCfvoDemo.xlsx");
        }
    }
}
```

### См. также

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


