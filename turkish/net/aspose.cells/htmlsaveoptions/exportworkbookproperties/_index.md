---
title: "HtmlSaveOptions.ExportWorkbookProperties"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Çalışma kitabı özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tır. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız varsayılan değeri koruyun."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportworkbookproperties/
---
## HtmlSaveOptions.ExportWorkbookProperties property

Çalışma kitabı özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

```csharp
public bool ExportWorkbookProperties { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorkbookPropertiesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabına bazı veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Çalışma kitabı özelliklerini ayarlayın
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Title";

            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // ExportWorkbookProperties'i false olarak ayarlayarak gösterin
            options.ExportWorkbookProperties = false;
            
            // Çalışma kitabını HTML olarak kaydet
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with ExportWorkbookProperties set to false");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


