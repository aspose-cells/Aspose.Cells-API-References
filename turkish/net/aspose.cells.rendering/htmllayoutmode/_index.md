---
title: "Enum HtmlLayoutMode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.HtmlLayoutMode enum'ı. HTML işleme için düzen modunu temsil eder"
type: docs
url: /tr/net/aspose.cells.rendering/htmllayoutmode/
---
## HtmlLayoutMode enumeration

HTML render'ı için düzen modunu temsil eder.

```csharp
public enum HtmlLayoutMode
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Normal | `0` | İçeriği MS Excel gibi işler. |
| Print | `1` | İçeriği yazdırma düzeni modunda işler. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassHtmlLayoutModeDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Çalışma sayfasına bazı örnek veriler ekleyin
                worksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");
                worksheet.Cells["A2"].PutValue("This demonstrates HtmlLayoutMode");

                // HtmlSaveOptions oluşturun ve düzen modunu Normal olarak ayarlayın
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                saveOptions.LayoutMode = HtmlLayoutMode.Normal;

                // Çalışma kitabını normal düzen modu ile kaydedin
                workbook.Save("NormalLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Normal layout mode.");

                // Düzen modunu Yazdırma olarak değiştirin
                saveOptions.LayoutMode = HtmlLayoutMode.Print;

                // Çalışma kitabını yazdırma düzen modu ile kaydedin
                workbook.Save("PrintLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Print layout mode.");

                // Enum değerlerini görüntüle
                Console.WriteLine($"Normal mode value: {HtmlLayoutMode.Normal}");
                Console.WriteLine($"Print mode value: {HtmlLayoutMode.Print}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HtmlLayoutMode: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


