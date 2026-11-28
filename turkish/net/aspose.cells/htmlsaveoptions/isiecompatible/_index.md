---
title: "HtmlSaveOptions.IsIECompatible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Çıktı HTML'nin IE tarayıcısıyla uyumlu olup olmadığını gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/isiecompatible/
---
## HtmlSaveOptions.IsIECompatible property

Çıktı HTML'nin IE tarayıcısıyla uyumlu olup olmadığını gösterir. Varsayılan değer false'tur.

```csharp
public bool IsIECompatible { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsIECompatibleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("HTML Export Demo");

            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // IsIECompatible özelliğini ayarla
            saveOptions.IsIECompatible = false; // Disable IE compatibility mode
            
            // Çalışma kitabını HTML seçenekleriyle kaydet
            workbook.Save("HtmlExportDemo.html", saveOptions);

            Console.WriteLine("HTML file saved with IsIECompatible = false");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


