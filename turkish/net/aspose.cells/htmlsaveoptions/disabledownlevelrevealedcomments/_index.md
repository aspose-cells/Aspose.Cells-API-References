---
title: "HtmlSaveOptions.DisableDownlevelRevealedComments"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Dosyayı html'ye dışa aktarırken Downlevelrevealed koşullu yorumların devre dışı bırakılıp bırakılmadığını gösterir, varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/
---
## HtmlSaveOptions.DisableDownlevelRevealedComments property

Dosya HTML'ye dışa aktarılırken Downlevel-revealed koşullu yorumların devre dışı bırakılıp bırakılmayacağını gösterir, varsayılan değer false'tur.

```csharp
public bool DisableDownlevelRevealedComments { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDisableDownlevelRevealedCommentsDemo
    {
        public static void Run()
        {
            // Yorumlu örnek bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a test comment";

            // DisableDownlevelRevealedComments ile HTML kaydetme seçeneklerini ayarla
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.DisableDownlevelRevealedComments = true;

            // Çalışma kitabını HTML seçenekleriyle kaydet
            workbook.Save("output.html", options);
            
            Console.WriteLine("Workbook saved with DisableDownlevelRevealedComments=true");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


