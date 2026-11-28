---
title: "PdfBookmarkEntry.DestinationName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfBookmarkEntry özelliği. Hedefin adını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering/pdfbookmarkentry/destinationname/
---
## PdfBookmarkEntry.DestinationName property

Hedefin adını alır veya ayarlar.

```csharp
public string DestinationName { get; set; }
```

### Açıklamalar

Eğer hedef adı ayarlanırsa, hedef bu adla adlandırılmış bir hedef olarak tanımlanır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfBookmarkEntryPropertyDestinationNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere örnek içerik ekleyin
            worksheet.Cells["A1"].PutValue("Primary Content Section");
            worksheet.Cells["A2"].PutValue("Secondary Content Section");

            // Ana PDF yer imi girdisi oluşturun
            PdfBookmarkEntry mainEntry = new PdfBookmarkEntry
            {
                Text = "Main Section",
                Destination = worksheet.Cells["A1"],
                IsOpen = true
            };

            // İlk DestinationName (null) okumasını göster
            Console.WriteLine($"Initial DestinationName: {mainEntry.DestinationName ?? "null"}");

            // Ana giriş için özel hedef adını ayarla
            mainEntry.DestinationName = "PrimaryDestination";
            Console.WriteLine($"Updated DestinationName: {mainEntry.DestinationName}");

            // Alt yer imi girişini oluştur
            PdfBookmarkEntry subEntry = new PdfBookmarkEntry
            {
                Text = "Sub Section",
                Destination = worksheet.Cells["A2"],
                DestinationName = "SecondaryDestination"
            };

            // Alt girişi ana yer imine ekle
            mainEntry.SubEntry = new System.Collections.ArrayList { subEntry };

            // Yer imi yapısıyla PDF kaydetme seçeneklerini yapılandır
            PdfSaveOptions pdfOptions = new PdfSaveOptions
            {
                Bookmark = mainEntry
            };

            // Çalışma kitabını PDF yer imleriyle kaydet
            workbook.Save("PdfBookmarkDestinationDemo.pdf", pdfOptions);

            Console.WriteLine("PDF created with custom bookmark destinations.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


