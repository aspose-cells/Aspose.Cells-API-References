---
title: "PaginatedSaveOptions.TextCrossType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. Metin genişliği hücre genişliğinden büyük olduğunda görüntüleme metin tipini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/textcrosstype/
---
## PaginatedSaveOptions.TextCrossType property

Metin genişliği hücre genişliğinden büyük olduğunda görüntüleme metin tipini alır veya ayarlar.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyTextCrossTypeDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücre sınırlarını aşacak uzun metin ayarlayın
            worksheet.Cells["A1"].PutValue("This is a long text that will cross cell boundaries");
            worksheet.Cells["B1"].PutValue("Another cell content");
            
            // Metnin hücreleri aşmasını sağlamak için sütun genişliğini ayarlayın
            worksheet.Cells.SetColumnWidth(0, 5);
            
            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions options = new PdfSaveOptions();
            
            // TextCrossType'ı CrossKeep olarak ayarlayarak gösterin
            options.TextCrossType = TextCrossType.CrossKeep;
            
            // Çalışma kitabını PDF olarak kaydedin
            workbook.Save("TextCrossTypeDemo.pdf", options);
            
            Console.WriteLine("PDF saved with TextCrossType.CrossKeep setting");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextCrossType](../../textcrosstype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


