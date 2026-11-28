---
title: "ImageOrPrintOptions.IsFontSubstitutionCharGranularity"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipinin değiştirilip değiştirilmediğini gösterir"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/
---
## ImageOrPrintOptions.IsFontSubstitutionCharGranularity property

Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipini değiştirmeyi gösterir.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### Açıklamalar

Varsayılan false'tur. Önce Çalışma Kitabı ve PdfSaveOption/sisteminin varsayılan yazı tipini hücre yazı tipi için deneyeceğiz.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyIsFontSubstitutionCharGranularityDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Potansiyel olarak desteklenmeyen bir yazı tipiyle hücreyi yapılandırın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with unavailable font");
            Style style = cell.GetStyle();
            style.Font.Name = "NonExistentFont";
            cell.SetStyle(style);

            // Görüntü renderleme seçeneklerini oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png, // Namespace reference now valid
                DefaultFont = "Arial",
                CheckWorkbookDefaultFont = false
            };

            // Özellik değerini görüntüleyin ve değiştirin
            Console.WriteLine($"Initial IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            
            // Varsayılan ayarla render edin
            new SheetRender(worksheet, options).ToImage(0, "BeforeFontSubstitutionChange.png");

            // Özelliği değiştirin ve tekrar render edin
            options.IsFontSubstitutionCharGranularity = true;
            Console.WriteLine($"Updated IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            new SheetRender(worksheet, options).ToImage(0, "AfterFontSubstitutionChange.png");

            // Referans için çalışma kitabını kaydedin
            workbook.Save("FontSubstitutionDemoWorkbook.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


