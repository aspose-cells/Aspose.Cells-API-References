---
title: "ColorScale.MaxCfvo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ColorScale. Получить или установить объект максимального значения этой шкалы цветов. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Min."
type: docs
url: /ru/net/aspose.cells/colorscale/maxcfvo/
---
## ColorScale.MaxCfvo property

Получить или установить объект максимального значения этого ColorScale. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Min.

```csharp
public ConditionalFormattingValue MaxCfvo { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMaxCfvoDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            ws.Cells["A1"].PutValue(1);
            ws.Cells["A2"].PutValue(2);
            ws.Cells["A3"].PutValue(3);
            ws.Cells["A4"].PutValue(4);
            ws.Cells["A5"].PutValue(5);

            int idx = ws.ConditionalFormattings.Add();
            FormatConditionCollection fcc = ws.ConditionalFormattings[idx];
            fcc.AddArea(CellArea.CreateCellArea("A1", "A5"));

            idx = fcc.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcc[idx];
            
            fc.ColorScale.Is3ColorScale = false;
            
            // Продемонстрировать использование свойства MaxCfvo
            fc.ColorScale.MaxCfvo.IsGTE = true;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Yellow;
            
            fc.ColorScale.MinCfvo.IsGTE = true;
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;

            workbook.Save("ColorScaleMaxCfvoDemo.xlsx");
        }
    }
}
```

### См. также

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


