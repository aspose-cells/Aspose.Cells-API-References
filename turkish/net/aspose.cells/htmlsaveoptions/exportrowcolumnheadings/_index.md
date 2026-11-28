---
title: "HtmlSaveOptions.ExportRowColumnHeadings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. HTML dosyalarına kaydederken sayfa satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportrowcolumnheadings/
---
## HtmlSaveOptions.ExportRowColumnHeadings property

Sayfanın satır ve sütun başlıklarının HTML dosyalarına kaydedilirken dışa aktarılıp aktarılmayacağını gösterir.

```csharp
public bool ExportRowColumnHeadings { get; set; }
```

### Açıklamalar

Varsayılan değer false'tur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportRowColumnHeadingsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);

            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // ExportRowColumnHeadings özelliğini false olarak ayarlayın (varsayılan true'tır)
            saveOptions.ExportRowColumnHeadings = false;

            // Başlıklar devre dışı bırakılmış halde çalışma kitabını kaydet
            workbook.Save("output_without_headings.html", saveOptions);

            // Şimdi başlıkları etkinleştir ve tekrar kaydet
            saveOptions.ExportRowColumnHeadings = true;
            workbook.Save("output_with_headings.html", saveOptions);

            Console.WriteLine("HTML files saved with different heading visibility settings.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


