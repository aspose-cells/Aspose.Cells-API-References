---
title: "Workbook.GetMatchingColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Mevcut palet içinde en uygun rengi bulun"
type: docs
url: /tr/net/aspose.cells/workbook/getmatchingcolor/
---
## Workbook.GetMatchingColor method

Mevcut palet içinde en iyi eşleşen Rengi bul.

```csharp
public Color GetMatchingColor(Color rawColor)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rawColor | Color | Ham renk. |

### Dönüş Değeri

En uygun renk.

### Açıklamalar

Excel 97-2003'te renk paletinde yalnızca 56 renk vardır. Renk palette yoksa, benzer bir renk ayarlanır.

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetMatchingColorWithColorDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Rengin palette olup olmadığını kontrol edin
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color testColor = Color.FromArgb(255, 123, 123, 123);
            Console.WriteLine("Is custom color in palette: " + workbook.IsColorInPalette(testColor));

            // Paletten eşleşen rengi al
            Color matchedColor = workbook.GetMatchingColor(testColor);
            Console.WriteLine($"Original color: R={testColor.R}, G={testColor.G}, B={testColor.B}");
            Console.WriteLine($"Matched color: R={matchedColor.R}, G={matchedColor.G}, B={matchedColor.B}");

            // Özel bir tema oluşturun
            Color[] themeColors = new Color[12];
            for (int i = 0; i < themeColors.Length; i++)
            {
                themeColors[i] = Color.FromArgb(255, 128 + i, 128 + i, 128 + i);
            }
            workbook.CustomTheme("CustomTheme", themeColors);

            // Tema rengini alın
            Color themeColor = workbook.GetThemeColor(ThemeColorType.FollowedHyperlink);
            Console.WriteLine($"Theme color: R={themeColor.R}, G={themeColor.G}, B={themeColor.B}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


