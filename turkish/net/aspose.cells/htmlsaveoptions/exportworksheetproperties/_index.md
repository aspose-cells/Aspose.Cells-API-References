---
title: "HtmlSaveOptions.ExportWorksheetProperties"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Çalışma sayfası özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız lütfen varsayılan değeri koruyun."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportworksheetproperties/
---
## HtmlSaveOptions.ExportWorksheetProperties property

Çalışma sayfası özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

```csharp
public bool ExportWorksheetProperties { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorksheetPropertiesDemo
    {
        public static void Run()
        {
            // Test verileriyle örnek bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // ExportWorksheetProperties devre dışı bırakılmış HTML kaydetme seçeneklerini ayarla
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportWorksheetProperties = false;
            
            // Çalışma sayfası özellikleri devre dışı bırakılmış şekilde kaydet
            workbook.Save("output_without_worksheet_props.html", options);

            // Çalışma sayfası özelliklerinin dışa aktarımını etkinleştir
            options.ExportWorksheetProperties = true;
            
            // Çalışma sayfası özellikleri etkinleştirilmiş şekilde kaydet
            workbook.Save("output_with_worksheet_props.html", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


