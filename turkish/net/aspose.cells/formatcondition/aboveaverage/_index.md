---
title: "FormatCondition.AboveAverage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition özelliği. Koşullu biçimlendirmelerin AboveAverage örneğini al. Varsayılan örnek kuralı, aralıktaki tüm değerlerin ortalamasının üzerindeki hücreleri vurgular. Yalnızca AboveAverage türü için geçerlidir."
type: docs
url: /tr/net/aspose.cells/formatcondition/aboveaverage/
---
## FormatCondition.AboveAverage property

Koşullu biçimlendirme'nin "AboveAverage" örneğini al. Varsayılan örneğin kuralı, aralıktaki tüm değerlerin ortalamasının üzerindeki hücreleri vurgular. Yalnızca type = AboveAverage için geçerlidir.

```csharp
public AboveAverage AboveAverage { get; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Ortalamanın üzerindeki koşullu biçimlendirmeyi ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 4, EndColumn = 0 });

            // Ortalamanın üzerindeki değerleri vurgulamak için ayarla
            FormatCondition fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = true;
            fc.Style.BackgroundColor = Color.Yellow;

            // Ortalamanın altındaki koşullu biçimlendirmeyi ekle
            index = worksheet.ConditionalFormattings.Add();
            fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 1, EndRow = 4, EndColumn = 1 });

            // Ortalamanın altındaki değerleri vurgulamak için ayarla
            fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = false;
            fc.Style.BackgroundColor = Color.LightBlue;

            // Çalışma kitabını kaydedin
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AboveAverage](../../aboveaverage/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


