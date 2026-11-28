---
title: "Workbook.IsColorInPalette"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Bir rengin elektronik tablo paletinde olup olmadığını kontrol eder"
type: docs
url: /tr/net/aspose.cells/workbook/iscolorinpalette/
---
## Workbook.IsColorInPalette method

Bir rengin elektronik tablo paletinde olup olmadığını kontrol eder.

```csharp
public bool IsColorInPalette(Color color)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color | Color | Renk yapısı. |

### Dönüş Değeri

Bu renk palette ise true döndürür. Aksi takdirde false döndürür

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodIsColorInPaletteWithColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Standart rengin palette olup olmadığını kontrol et
            bool isRedInPalette = workbook.IsColorInPalette(Color.Red);
            Console.WriteLine("Is Red in palette: " + isRedInPalette);
            
            // Özel rengin palette olup olmadığını kontrol et
            Color customColor = Color.FromArgb(255, 123, 123, 123);
            bool isCustomInPalette = workbook.IsColorInPalette(customColor);
            Console.WriteLine("Is custom color in palette: " + isCustomInPalette);
            
            // Paletten eşleşen rengi al
            Color matchedColor = workbook.GetMatchingColor(customColor);
            Console.WriteLine("Matched color R value: " + matchedColor.R);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


