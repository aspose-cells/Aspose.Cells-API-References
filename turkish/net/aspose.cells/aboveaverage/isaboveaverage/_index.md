---
title: "AboveAverage.IsAboveAverage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AboveAverage özelliği. Kuralın ortalamanın üzerindeki bir kural olup olmadığını belirten bayrağı alır veya ayarlar. true değeri, ortalamanın üzeri olduğunu gösterir. Varsayılan değer true'tır."
type: docs
url: /tr/net/aspose.cells/aboveaverage/isaboveaverage/
---
## AboveAverage.IsAboveAverage property

Kuralın "ortalamanın üzeri" kuralı olup olmadığını gösteren bayrağı alır veya ayarlar. 'true' 'ortalamanın üzeri' anlamına gelir. Varsayılan değer true'dur.

```csharp
public bool IsAboveAverage { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsAboveAverageDemo
    {
        public static void Run()
        {
            // Yeni bir Workbook oluşturun
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasını al
            Worksheet worksheet = workbook.Worksheets[0];

            // Koşullu biçimlendirmeyi göstermek için örnek veri ekle
            for (int i = 0; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Koşullu biçimlendirme ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme aralığını ayarla
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Bir AboveAverage koşulu ekle
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // AboveAverage özelliklerini yapılandır
            fc.AboveAverage.IsAboveAverage = true;  // Highlight values above average
            fc.AboveAverage.IsEqualAverage = false; // Exclude values equal to average

            // Excel dosyasını kaydet
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


