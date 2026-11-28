---
title: "Sınıf ColorScale"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ColorScale sınıfı. ColorScale koşullu biçimlendirme kuralını tanımlar. Bu koşullu biçimlendirme kuralı hücrelerde kademeli bir renk ölçeği oluşturur"
type: docs
url: /tr/net/aspose.cells/colorscale/
---
## ColorScale class

ColorScale koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı hücrelerde kademeli bir renk ölçeği oluşturur.

```csharp
public class ColorScale
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Is3ColorScale](../../aspose.cells/colorscale/is3colorscale/) { get; set; } | Koşullu biçimlendirmenin 3 renk ölçeği olup olmadığını gösterir. |
| [MaxCfvo](../../aspose.cells/colorscale/maxcfvo/) { get; } | Bu ColorScale'in maksimum değer nesnesini alın veya ayarlayın. Null veya FormatConditionValueType.Min tipinde CFValueObject atanamaz. |
| [MaxColor](../../aspose.cells/colorscale/maxcolor/) { get; set; } | Aralıktaki maksimum değer için geçiş rengini alın veya ayarlayın. |
| [MidCfvo](../../aspose.cells/colorscale/midcfvo/) { get; } | Bu ColorScale'in orta değer nesnesini alın veya ayarlayın. FormatConditionValueType.Max veya FormatConditionValueType.Min tipinde CFValueObject atanamaz. |
| [MidColor](../../aspose.cells/colorscale/midcolor/) { get; set; } | Aralıktaki orta değer için geçiş rengini alın veya ayarlayın. |
| [MinCfvo](../../aspose.cells/colorscale/mincfvo/) { get; } | Bu ColorScale'in minimum değer nesnesini alın veya ayarlayın. Null veya FormatConditionValueType.Max tipinde CFValueObject atanamaz. |
| [MinColor](../../aspose.cells/colorscale/mincolor/) { get; set; } | Aralıktaki minimum değer için geçiş rengini alın veya ayarlayın. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColorScaleDemo
    {
        public static void ColorScaleExample()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı örnek veriler ekleyin
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            // Koşullu biçimlendirme kuralı ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 9 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // ColorScale nesnesine erişin
            ColorScale colorScale = fc.ColorScale;

            // ColorScale için özellikleri ayarlayın
            colorScale.Is3ColorScale = true;
            colorScale.MinColor = Color.Green;
            colorScale.MidColor = Color.Yellow;
            colorScale.MaxColor = Color.Red;

            // Minimum, orta ve maksimum değer nesnelerini ayarlayın
            ConditionalFormattingValue minCfvo = colorScale.MinCfvo;
            minCfvo.Type = FormatConditionValueType.Min;
            minCfvo.Value = null;

            ConditionalFormattingValue midCfvo = colorScale.MidCfvo;
            midCfvo.Type = FormatConditionValueType.Percentile;
            midCfvo.Value = 50;

            ConditionalFormattingValue maxCfvo = colorScale.MaxCfvo;
            maxCfvo.Type = FormatConditionValueType.Max;
            maxCfvo.Value = null;

            // Çalışma kitabını kaydedin
            workbook.Save("ColorScaleExample.xlsx");
            workbook.Save("ColorScaleExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


