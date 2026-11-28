---
title: "CopyOptions.ReferToDestinationSheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CopyOptions özelliği. Aynı dosyada aralık kopyalanırken ve grafik kaynak sayfaya başvuruyorsa False, kopyalanan grafiğin veri kaynağının değişmeyeceği anlamına gelir. True ise kopyalanan grafiğin veri kaynağının hedef sayfaya başvuracağı anlamına gelir."
type: docs
url: /tr/net/aspose.cells/copyoptions/refertodestinationsheet/
---
## CopyOptions.ReferToDestinationSheet property

Aynı dosyada aralık kopyalanırken ve grafik kaynak sayfaya referans veriyorsa, False kopyalanan grafiğin veri kaynağının değişmeyeceği anlamına gelir. True ise kopyalanan grafiğin veri kaynağının hedef sayfaya referans vereceği anlamına gelir.

```csharp
public bool ReferToDestinationSheet { get; set; }
```

### Açıklamalar

Varsayılan değer false'tur, MS Excel gibi çalışır. Örneğin: veri kaynağı "sheet1!A1:B10" olan bir grafiği "sheet1" çalışma sayfasından başka bir "sheet2" çalışma sayfasına kopyalıyorsanız, veri kaynağı "sheet2!A1:B10" olarak değişecektir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToDestinationSheetDemo
    {
        public static void Run()
        {
            // Örnek veri içeren kaynak çalışma kitabını oluşturun
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B1"].PutValue(100);
            sourceSheet.Cells["A2"].PutValue("=SUM(B1)");

            // Hedef çalışma kitabı oluştur
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets.Add("DestinationSheet");

            // ReferToDestinationSheet ile kopyalama seçeneklerini ayarlayın
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ReferToDestinationSheet = true;

            // Seçeneklerle çalışma sayfasını kopyalayın
            destSheet.Copy(sourceSheet, copyOptions);

            // Sonucu kaydet
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


