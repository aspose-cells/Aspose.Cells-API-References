---
title: "FillFormat.PresetColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FillFormat özelliği. Belirtilen doldurma için gradyan ön ayar rengini döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/fillformat/presetcolor/
---
## FillFormat.PresetColor property

Belirtilen dolgu için gradient ön ayar rengini döndürür.

```csharp
public GradientPresetType PresetColor { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPresetColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik alanının doldurma biçimine erişin
            FillFormat fillFormat = chart.ChartArea.Area.FillFormat;

            // Bir gradyan ön ayar rengi ayarlayın
            fillFormat.SetPresetColorGradient(GradientPresetType.Ocean, GradientStyleType.DiagonalUp, 2);

            // Ön ayar rengini görüntüleyin ve doğrulayın
            Console.WriteLine("Preset Color: " + fillFormat.PresetColor);

            // Çalışma kitabını kaydedin
            workbook.Save("FillFormatPresetColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [GradientPresetType](../../gradientpresettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


