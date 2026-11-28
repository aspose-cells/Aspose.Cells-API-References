---
title: "HtmlSaveOptions.LayoutMode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. HTML'ye kaydederken düzen modunu alır veya ayarlar. Varsayılan değer Normal."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/layoutmode/
---
## HtmlSaveOptions.LayoutMode property

HTML olarak kaydederken düzen modunu alır veya ayarlar. Varsayılan değer Normal'dir.

```csharp
public HtmlLayoutMode LayoutMode { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyLayoutModeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Layout Mode Test");

            try
            {
                // HtmlSaveOptions örneği oluştur
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Mevcut LayoutMode değerini göster
                Console.WriteLine("Current LayoutMode: " + options.LayoutMode);

                // LayoutMode'u Print olarak ayarla
                options.LayoutMode = HtmlLayoutMode.Print;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Çalışma kitabını Print düzen modu ile kaydet
                workbook.Save("LayoutModePrint.html", options);

                // LayoutMode'u Normal olarak ayarla
                options.LayoutMode = HtmlLayoutMode.Normal;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Çalışma kitabını Normal düzen modu ile kaydet
                workbook.Save("LayoutModeNormal.html", options);

                Console.WriteLine("HTML files saved with different LayoutMode settings.");
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

* enum [HtmlLayoutMode](../../../aspose.cells.rendering/htmllayoutmode/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


