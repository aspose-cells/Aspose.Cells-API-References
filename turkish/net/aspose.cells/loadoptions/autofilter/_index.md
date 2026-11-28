---
title: "LoadOptions.AutoFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/loadoptions/autofilter/
---
## LoadOptions.AutoFilter property

Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmeyeceğini gösterir.

```csharp
public bool AutoFilter { get; set; }
```

### Açıklamalar

Bazen otomatik filtre ayarlı olsa da, ilgili satırlar dosyada gizlenmez. Şimdi yalnızca SpreadSheetML dosyası için çalışıyor.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Yükleme seçenekleri oluşturun ve AutoFilter'ı etkinleştirin
            LoadOptions options = new LoadOptions();
            options.AutoFilter = true;

            // AutoFilter etkinleştirilmiş şekilde çalışma kitabını yükleyin
            Workbook workbook = new Workbook("example.xlsx", options);

            // İlk çalışma sayfasına erişin ve AutoFilter uygulayın
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = "A1:D10";
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


