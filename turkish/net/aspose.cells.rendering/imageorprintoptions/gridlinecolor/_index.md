---
title: "ImageOrPrintOptions.GridlineColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Izgara çizgi rengini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/gridlinecolor/
---
## ImageOrPrintOptions.GridlineColor property

Izgara çizgi rengini alır veya ayarlar.

```csharp
public Color GridlineColor { get; set; }
```

### Açıklamalar

Kaynak dosyadaki ızgara çizgi rengi ayarlarını yok sayacaktır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasının içeriğe sahip olması için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Demo for GridlineColor property");

            try
            {
                // ImageOrPrintOptions bir örnek oluşturun
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Mevcut GridlineColor değerini göster (yalnızca‑okunur veya okuma/yazma)
                // Özellik tipi System.Drawing.Color olarak varsayılır
                Console.WriteLine("Current GridlineColor: " + options.GridlineColor);

                // İsteğe bağlı olarak sayfayı bir görüntüye renderlayarak varsayılan ızgara çizgi renginin etkisini görebilirsiniz
                // (Değeri değiştirmenize gerek yok; sadece kullanımını gösteriyoruz.)
                SheetRender renderer = new SheetRender(worksheet, options);
                renderer.ToImage(0, "GridlineColorDemo.png");

                // Çalışma kitabını kaydedin (isteğe bağlı)
                workbook.Save("GridlineColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during demo: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


