---
title: "HtmlSaveOptions.ExportCellCoordinate"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Dosya html olarak kaydedilirken boş olmayan hücrelerin excel koordinatının dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. Çıktı html'yi excel'e içe aktarmak istiyorsanız lütfen varsayılan değeri koruyun"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportcellcoordinate/
---
## HtmlSaveOptions.ExportCellCoordinate property

Dosya HTML olarak kaydedilirken boş olmayan hücrelerin Excel koordinatlarının dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. Çıktı HTML'yi Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

```csharp
public bool ExportCellCoordinate { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCellCoordinateDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // HTML kaydetme seçeneklerini oluşturun ve ExportCellCoordinate özelliğini etkinleştirin
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportCellCoordinate = true;

            // Çalışma kitabını hücre koordinatlarıyla HTML olarak kaydedin
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with cell coordinates exported successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


