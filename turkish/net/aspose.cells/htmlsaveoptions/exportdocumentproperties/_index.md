---
title: "HtmlSaveOptions.ExportDocumentProperties"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız lütfen varsayılan değeri koruyun"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportdocumentproperties/
---
## HtmlSaveOptions.ExportDocumentProperties property

Belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

```csharp
public bool ExportDocumentProperties { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı belge özellikleri ekleyin
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Örnek hücre verileri ekleyin
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // HTML kaydetme seçeneklerini oluşturun ve ExportDocumentProperties'i false olarak ayarlayın
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportDocumentProperties = false;
            
            // Çalışma kitabını HTML olarak kaydet
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with document properties export disabled.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


