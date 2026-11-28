---
title: "HtmlSaveOptions.IsMobileCompatible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Çıktı HTML'sinin mobil cihazlarla uyumlu olup olmadığını gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/ismobilecompatible/
---
## HtmlSaveOptions.IsMobileCompatible property

Çıktı HTML'nin mobil cihazlarla uyumlu olup olmadığını gösterir. Varsayılan değer false'tur.

```csharp
public bool IsMobileCompatible { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsMobileCompatibleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Mobile Compatibility Test");

            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Mobil uyumluluğu ayarlayın
            saveOptions.IsMobileCompatible = true;

            // Mobil uyumluluk etkinleştirilmiş şekilde kaydedin
            workbook.Save("MobileCompatible.html", saveOptions);

            // Mobil uyumlu olmayan olarak değiştirin
            saveOptions.IsMobileCompatible = false;
            workbook.Save("NonMobileCompatible.html", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


