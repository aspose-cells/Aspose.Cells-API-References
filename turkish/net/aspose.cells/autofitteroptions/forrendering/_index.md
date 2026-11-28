---
title: "AutoFitterOptions.ForRendering"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFitterOptions özelliği. Render amaçlı uyum sağlayıp sağlamadığını gösterir"
type: docs
url: /tr/net/aspose.cells/autofitteroptions/forrendering/
---
## AutoFitterOptions.ForRendering property

Render amacı için uyumlu olup olmadığını gösterir.

```csharp
public bool ForRendering { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyForRenderingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Uzun metinle örnek veri ayarla
            worksheet.Cells["A1"].PutValue("This is a long text that needs auto-fitting for rendering purposes.");
            
            // AutoFitterOptions oluştur ve ForRendering'i true olarak ayarla
            AutoFitterOptions options = new AutoFitterOptions();
            options.ForRendering = true;

            // Render dikkate alınarak satırı otomatik olarak uyarla
            worksheet.AutoFitRows(0, 0, options);

            // Sonuçta oluşan satır yüksekliğini piksel olarak çıktı ver
            Console.WriteLine("Row height after auto-fitting (pixels): " + worksheet.Cells.GetRowHeightPixel(0));
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


