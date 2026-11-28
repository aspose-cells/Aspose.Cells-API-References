---
title: "MarkdownSaveOptions.SplitTablesByBlankRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MarkdownSaveOptions özelliği. Çalışma sayfasındaki boş satırların Markdown'a dışa aktarılırken tablo ayırıcıları olarak ele alınıp alınmayacağını gösterir. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/markdownsaveoptions/splittablesbyblankrow/
---
## MarkdownSaveOptions.SplitTablesByBlankRow property

Çalışma sayfasındaki boş satırların Markdown'a dışa aktarılırken tablo ayırıcıları olarak ele alınıp alınmayacağını gösterir. Varsayılan değer false'tur.

```csharp
public bool SplitTablesByBlankRow { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertySplitTablesByBlankRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tablo bölmeyi göstermek için boş satırlarla örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Table 1 Header";
            worksheet.Cells["B1"].Value = "Value 1";
            worksheet.Cells["A2"].Value = "Data 1";
            worksheet.Cells["B2"].Value = "Data 2";

            // Boş bir satır ekleyin (satır 3)
            worksheet.Cells["A4"].Value = "Table 2 Header";
            worksheet.Cells["B4"].Value = "Value 2";
            worksheet.Cells["A5"].Value = "Data 3";
            worksheet.Cells["B5"].Value = "Data 4";

            // MarkdownSaveOptions örneği oluştur
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Varsayılan SplitTablesByBlankRow değerini gösterin
                Console.WriteLine("Default SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // Tabloları boş satırlarla bölmek için SplitTablesByBlankRow değerini true olarak ayarlayın
                saveOptions.SplitTablesByBlankRow = true;

                // Güncellenmiş değeri gösterin
                Console.WriteLine("Updated SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // Tablo bölme etkinleştirilmiş şekilde çalışma kitabını markdown olarak kaydedin
                workbook.Save("SplitTablesByBlankRowDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with table splitting by blank rows enabled.");
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


