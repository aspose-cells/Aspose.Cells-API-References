---
title: "AboveAverage.StdDev"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AboveAverage özelliği. Koşullu biçimlendirme kuralında ortalamanın üstünde veya altında dahil edilecek standart sapma sayısını alır veya ayarlar. Giriş değeri 0 ile 3 arasında olmalıdır, 0 ve 3 dahil. Bu değeri 0 olarak ayarlamak, stdDev'in ayarlanmadığı anlamına gelir. Varsayılan değer 0'dır."
type: docs
url: /tr/net/aspose.cells/aboveaverage/stddev/
---
## AboveAverage.StdDev property

Koşullu biçimlendirme kuralında ortalamanın üzerindeki veya altındaki standart sapma sayısını alır veya ayarlar. Giriş değeri 0 ile 3 arasında olmalıdır (0 ve 3 dahil). Bu değeri 0 olarak ayarlamak, stdDev'in ayarlanmadığı anlamına gelir. Varsayılan değer 0'dır.

```csharp
public int StdDev { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyStdDevDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            CellArea ca = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.StdDev = 2;

            // Örnek verileri doldur
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50;

            workbook.Save("AboveAverageStdDevDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


