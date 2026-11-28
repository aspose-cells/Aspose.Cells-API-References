---
title: "AboveAverage.IsEqualAverage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AboveAverage özelliği. aboveAverage ve belowAverage kriterlerinin ortalamayı kendisi dahil edip etmeyeceğini belirten bayrağı alır veya ayarlar. true değeri, ortalama değerinin kriterde dahil edileceğini gösterir. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/aboveaverage/isequalaverage/
---
## AboveAverage.IsEqualAverage property

‘aboveAverage’ ve ‘belowAverage’ kriterlerinin ortalamayı kendisi dahil edip etmeyeceğini gösteren bayrağı alır veya ayarlar. 'true' ortalama değerinin kriterlere dahil edilmesini gösterir. Varsayılan değer false'tur.

```csharp
public bool IsEqualAverage { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsEqualAverageDemo
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
            fc.Style.BackgroundColor = Color.LightBlue;

            // IsEqualAverage özelliğini göster
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false; // Cells equal to average won't be formatted

            // Örnek verileri doldur
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50; // Average is 30

            workbook.Save("AboveAverageIsEqualAverageDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


