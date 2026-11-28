---
title: "ColorScale.MinCfvo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ColorScale özelliği. Bu ColorScale'in minimum değer nesnesini alır veya ayarlar. Null veya FormatConditionValueType.Max tipinde CFValueObject atanamaz"
type: docs
url: /tr/net/aspose.cells/colorscale/mincfvo/
---
## ColorScale.MinCfvo property

Bu ColorScale'in minimum değer nesnesini alın veya ayarlayın. Null veya FormatConditionValueType.Max tipinde CFValueObject atanamaz.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Bir renk ölçeği koşullu biçimlendirme oluştur
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Renk ölçeği ekle
            int csIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            ColorScale cs = fcc[csIndex].ColorScale;

            // MinCfvo özelliklerini ayarla
            cs.MinCfvo.Type = FormatConditionValueType.Min;
            cs.MinCfvo.Value = "0";
            cs.MinColor = System.Drawing.Color.Red;

            // MidCfvo özelliklerini ayarla
            cs.MidCfvo.Type = FormatConditionValueType.Percentile;
            cs.MidCfvo.Value = "50";
            cs.MidColor = System.Drawing.Color.Yellow;

            // MaxCfvo özelliklerini ayarla
            cs.MaxCfvo.Type = FormatConditionValueType.Max;
            cs.MaxCfvo.Value = "0";
            cs.MaxColor = System.Drawing.Color.Green;

            // Çalışma kitabını kaydedin
            workbook.Save("ColorScaleMinCfvoDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


