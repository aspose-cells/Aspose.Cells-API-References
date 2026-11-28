---
title: "SaveOptions.MergeAreas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SaveOptions özelliği. Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir."
type: docs
url: /tr/net/aspose.cells/saveoptions/mergeareas/
---
## SaveOptions.MergeAreas property

Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir.

```csharp
public bool MergeAreas { get; set; }
```

### Açıklamalar

Varsayılan değer false'tur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyMergeAreasDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Verileri doldurun ve birleştirilmiş hücreler oluşturun.
            worksheet.Cells["A1"].PutValue("Merged Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // A1:B1 hücrelerini birleştirin.
            worksheet.Cells.Merge(0, 0, 1, 2);

            // MergeAreas etkinleştirilmiş kaydetme seçenekleri oluşturun.
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MergeAreas = true;

            // Birleştirilmiş alan optimizasyonu ile kaydedin.
            workbook.Save("MergeAreasDemo.xlsx", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


