---
title: "MarkdownSaveOptions.AlignColumnPadding"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MarkdownSaveOptions özelliği. Oluşturulan Markdown tabloları için sütun hizalamasının etkin olup olmadığını gösterir. Etkin olduğunda sütunlar, hücre içeriğini belirtilen karakterle (genellikle boşluk) doldurarak hizalanır. Sütun hizalamasını devre dışı bırakmak için 0 olarak ayarlayın varsayılan"
type: docs
url: /tr/net/aspose.cells/markdownsaveoptions/aligncolumnpadding/
---
## MarkdownSaveOptions.AlignColumnPadding property

Oluşturulan Markdown tabloları için sütun hizalamasının etkin olup olmadığını gösterir. Etkinleştirildiğinde, sütunlar belirtilen karakterle (genellikle boşluk için ' ') hücre içeriği doldurularak hizalanır. Sütun hizalamasını devre dışı bırakmak için '\\0' olarak ayarlayın (varsayılan).

```csharp
public char AlignColumnPadding { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyAlignColumnPaddingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sütun hizalamasını göstermek için örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "1.99";
            worksheet.Cells["C2"].Value = "10";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = "0.99";
            worksheet.Cells["C3"].Value = "20";

            // MarkdownSaveOptions örneği oluştur
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Varsayılan AlignColumnPadding değerini göster
                Console.WriteLine("Default AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Sütun hizalaması için AlignColumnPadding'i boşluk karakterine ayarlayın
                saveOptions.AlignColumnPadding = ' ';

                // Güncellenmiş değeri gösterin
                Console.WriteLine("Updated AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Çalışma kitabını sütun hizalamasıyla markdown olarak kaydedin
                workbook.Save("AlignColumnPaddingDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with column alignment enabled.");
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


