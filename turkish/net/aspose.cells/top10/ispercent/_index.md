---
title: "Top10.IsPercent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Top10 özelliği. Bir üst/alt n kuralının üst/alt n yüzde kuralı olup olmadığını alır veya ayarlar. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/top10/ispercent/
---
## Top10.IsPercent property

\"top/bottom n\" kuralının \"top/bottom n percent\" kuralı olup olmadığını alın veya ayarlayın. Varsayılan değer false.

```csharp
public bool IsPercent { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10PropertyIsPercentDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Bir Top10 koşullu biçimlendirme kuralı ekleyin
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.Top10, OperatorType.None, null, null);

            // Top10 biçim koşulunu al
            FormatCondition fc = fcc[0];
            
            // Top10 özelliklerini ayarla
            fc.Top10.IsPercent = true;  // Demonstrate IsPercent property
            fc.Top10.IsBottom = false;
            fc.Top10.Rank = 3;

            // Biçimlendirme stilini uygulayın
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // Çalışma kitabını kaydedin
            workbook.Save("Top10IsPercentDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


