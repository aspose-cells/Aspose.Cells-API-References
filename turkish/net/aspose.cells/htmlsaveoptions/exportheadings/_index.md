---
title: "HtmlSaveOptions.ExportHeadings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. HTML dosyalarına kaydederken sayfa satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportheadings/
---
## HtmlSaveOptions.ExportHeadings property

Sayfanın satır ve sütun başlıklarının HTML dosyalarına kaydedilirken dışa aktarılıp aktarılmayacağını gösterir.

```csharp
[Obsolete("Use HtmlSaveOptions.ExportRowColumnHeadings instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExportHeadings { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen HtmlSaveOptions.ExportRowColumnHeadings özelliğini kullanın. Bu özellik, Haziran 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportHeadingsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // HTML kaydetme seçeneklerini oluşturun ve başlıkların dışa aktarımını etkinleştirin
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportHeadings = true;

            // Başlıklarla HTML olarak kaydedin
            workbook.Save("output_with_headings.html", options);
            
            // Karşılaştırma için başlıklar olmadan tekrar kaydedin
            options.ExportHeadings = false;
            workbook.Save("output_without_headings.html", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


