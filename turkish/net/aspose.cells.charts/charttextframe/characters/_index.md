---
title: "ChartTextFrame.Characters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartTextFrame yöntemi. Metin içinde bir karakter aralığını temsil eden bir Characters nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells.charts/charttextframe/characters/
---
## ChartTextFrame.Characters method

Metin içindeki bir karakter aralığını temsil eden Characters nesnesini döndürür

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | Int32 | Karakterin başlangıç indeksidir. |
| uzunluk | Int32 | Karakter sayısı. |

### Dönüş Değeri

Karakterler nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFrameMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Grafik oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Veri etiketlerine erişin ve belirli karakterler için yazı tipi boyutunu ayarlayın
            chart.NSeries[0].Points[0].DataLabels.ShowValue = true;
            chart.NSeries[0].Points[0].DataLabels.Characters(0, 5).Font.Size = 14;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


