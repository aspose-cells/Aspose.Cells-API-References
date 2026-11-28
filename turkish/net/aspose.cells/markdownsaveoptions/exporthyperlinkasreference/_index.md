---
title: "MarkdownSaveOptions.ExportHyperlinkAsReference"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MarkdownSaveOptions özelliği. Hipermetin bağlantısını satır içi biçim yerine referans tanımlarıyla dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/markdownsaveoptions/exporthyperlinkasreference/
---
## MarkdownSaveOptions.ExportHyperlinkAsReference property

Hipermetin bağlantısını satır içi biçim yerine referans tanımlarıyla dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

```csharp
public bool ExportHyperlinkAsReference { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportHyperlinkAsReferenceDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Bir hücreye örnek metin koyun
            sheet.Cells["A1"].PutValue("Visit Aspose");

            // Hücreye (A1) bir hipermetin bağlantısı ekleyin
            // Parametreler: firstRow, firstColumn, totalRows, totalColumns, hyperlink
            sheet.Hyperlinks.Add(0, 0, 1, 1, "https://www.aspose.com");

            // Markdown kaydetme seçeneklerini başlatın
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Bu demoda ExportHyperlinkAsReference özelliğine doğrudan erişin (yalnızca okunur)
                Console.WriteLine("ExportHyperlinkAsReference value: " + saveOptions.ExportHyperlinkAsReference);

                // Çalışma kitabını markdown olarak kaydedin; özellik (true ise) hipermetin bağlantılarının dışa aktarım şeklini etkiler
                workbook.Save("ExportHyperlinkAsReferenceDemo.md", saveOptions);
                Console.WriteLine("Workbook saved as markdown.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


