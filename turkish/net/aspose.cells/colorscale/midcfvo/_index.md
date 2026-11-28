---
title: "ColorScale.MidCfvo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ColorScale özelliği. Bu ColorScale'in orta değer nesnesini alır veya ayarlar. FormatConditionValueType.Max veya FormatConditionValueType.Min tipinde CFValueObject atanamaz"
type: docs
url: /tr/net/aspose.cells/colorscale/midcfvo/
---
## ColorScale.MidCfvo property

Bu ColorScale'in orta değer nesnesini alın veya ayarlayın. FormatConditionValueType.Max veya FormatConditionValueType.Min tipinde CFValueObject atanamaz.

```csharp
public ConditionalFormattingValue MidCfvo { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMidCfvoDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // Bir renk ölçeği koşullu biçimlendirme ekle
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            int conditionIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            
            // Renk ölçeği için orta nokta değerini ayarla
            ColorScale colorScale = fcc[conditionIndex].ColorScale;
            colorScale.MidCfvo.Type = FormatConditionValueType.Number;
            colorScale.MidCfvo.Value = 50;

            // Çalışma kitabını kaydedin
            workbook.Save("ColorScalePropertyMidCfvoDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


