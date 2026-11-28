---
title: "FormatCondition.ColorScale"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition özelliği. Koşullu biçimlendirmelerin ColorScale örneğini alır. Varsayılan örnek yeşil-sarı-kırmızı bir 3ColorScale'tir. Yalnızca ColorScale türü için geçerlidir."
type: docs
url: /tr/net/aspose.cells/formatcondition/colorscale/
---
## FormatCondition.ColorScale property

Koşullu biçimlendirme'nin "ColorScale" örneğini al. Varsayılan örnek, "yeşil-sarı-kırmızı" 3ColorScale'dir. Yalnızca type = ColorScale için geçerlidir.

```csharp
public ColorScale ColorScale { get; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Bir renk ölçeği koşullu biçimlendirme ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Koşullu biçimlendirme için aralığı ayarla
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Renk ölçeği özelliklerini ayarla
            fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[0];
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Green;

            // Çalışma kitabını kaydedin
            workbook.Save("ColorScaleExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ColorScale](../../colorscale/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


