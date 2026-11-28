---
title: "DocxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocxSaveOptions özelliği. Bir xlsx dosyasının grafik veri kaynağı olarak gömülüp gömülmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/docxsaveoptions/embedxlsxaschartdatasource/
---
## DocxSaveOptions.EmbedXlsxAsChartDataSource property

Grafiğin veri kaynağı olarak bir xlsx dosyasının gömülüp gömülmediğini gösterir.

```csharp
public bool EmbedXlsxAsChartDataSource { get; set; }
```

### Açıklamalar

Varsayılan değer true'tur.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına erişin ve örnek veri ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Chart Data";

            try
            {
                // DocxSaveOptions'ı başlatın
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // EmbedXlsxAsChartDataSource özelliğinin varsayılan değerini göster
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Kullanımını göstermek için EmbedXlsxAsChartDataSource'ı true olarak ayarla
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Çalışma kitabını yapılandırılmış seçeneklerle DOCX olarak kaydedin
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with EmbedXlsxAsChartDataSource option.");
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

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


