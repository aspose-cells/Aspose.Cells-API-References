---
title: "Sınıf AboveAverage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.AboveAverage sınıfı. AboveAverage koşullu biçimlendirme kuralını açıklar. Bu koşullu biçimlendirme kuralı, aralıktaki tüm değerlerin ortalamasının üzerinde veya altında olan hücreleri vurgular."
type: docs
url: /tr/net/aspose.cells/aboveaverage/
---
## AboveAverage class

AboveAverage koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı, aralıktaki tüm değerlerin ortalamasının üzerindeki veya altındaki hücreleri vurgular.

```csharp
public class AboveAverage
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [AboveAverage](aboveaverage/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [IsAboveAverage](../../aspose.cells/aboveaverage/isaboveaverage/) { get; set; } | Kuralın "ortalamanın üzeri" kuralı olup olmadığını gösteren bayrağı alır veya ayarlar. 'true' 'ortalamanın üzeri' anlamına gelir. Varsayılan değer true'dur. |
| [IsEqualAverage](../../aspose.cells/aboveaverage/isequalaverage/) { get; set; } | ‘aboveAverage’ ve ‘belowAverage’ kriterlerinin ortalamayı kendisi dahil edip etmeyeceğini gösteren bayrağı alır veya ayarlar. 'true' ortalama değerinin kriterlere dahil edilmesini gösterir. Varsayılan değer false'tur. |
| [StdDev](../../aspose.cells/aboveaverage/stddev/) { get; set; } | Koşullu biçimlendirme kuralında ortalamanın üzerindeki veya altındaki standart sapma sayısını alır veya ayarlar. Giriş değeri 0 ile 3 arasında olmalıdır (0 ve 3 dahil). Bu değeri 0 olarak ayarlamak, stdDev'in ayarlanmadığı anlamına gelir. Varsayılan değer 0'dır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class AboveAverageDemo
    {
        public static void AboveAverageExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            // Çalışma sayfasına bir koşullu biçimlendirme koleksiyonu ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            // Koşullu biçimlendirmeyi uygulamak için hücre alanını tanımla
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Koleksiyona bir ortalamanın üzeri koşulu ekle
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            // Koşul için arka plan rengini ayarla
            fc.Style.BackgroundColor = Color.Yellow;

            // Ortalamanın üzeri koşulu için özellikleri ayarla
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            Cells cells = worksheet.Cells;
            cells["A1"].Value = 20;
            cells["A2"].Value = 300;
            cells["A3"].Value = 40;
            cells["A4"].Value = 500;
            cells["A5"].Value = 6;
            cells["A6"].Value = 70;
            cells["A7"].Value = 8;
            cells["A8"].Value = 900;
            cells["A9"].Value = 10;

            cells["C1"].Value = 2;
            cells["C2"].Value = 3;
            cells["C3"].Value = 4;
            cells["C4"].Value = 5;
            cells["C5"].Value = 3;
            cells["C6"].Value = 2;
            cells["C7"].Value = 8;
            cells["C8"].Value = 300;
            cells["C9"].Value = 10;

            // Çalışma kitabını kaydedin
            workbook.Save("AboveAverageExample.xlsx");
            workbook.Save("AboveAverageExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


