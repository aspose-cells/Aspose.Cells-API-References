---
title: "HtmlSaveOptions.ExportCommentsType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Yorumların html dosyalarına aktarım tipini temsil eder."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportcommentstype/
---
## HtmlSaveOptions.ExportCommentsType property

Yorumların HTML dosyalarına dışa aktarım türünü temsil eder.

```csharp
public PrintCommentsType ExportCommentsType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCommentsTypeDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücre adı kullanarak örnek yorum ekleyin
            Comment comment = worksheet.Comments["A1"];
            comment.Note = "This is a test comment";
            
            // ExportCommentsType ile HTML kaydetme seçeneklerini ayarlayın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportCommentsType = PrintCommentsType.PrintInPlace;
            
            // HTML olarak kaydet
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file with comments exported successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PrintCommentsType](../../printcommentstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


