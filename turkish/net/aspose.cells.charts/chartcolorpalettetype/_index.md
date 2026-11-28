---
title: "Enum ChartColorPaletteType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.ChartColorPaletteType enum. Excel grafiğinde kullanılan tüm Monochromatic Paletleri listeler."
type: docs
url: /tr/net/aspose.cells.charts/chartcolorpalettetype/
---
## ChartColorPaletteType enumeration

Excel grafiğinde kullanılan tüm Monochromatic Palettes'i sıralar.

```csharp
public enum ChartColorPaletteType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| MonochromaticPalette1 | `1` | accent1 tema renk geçişi, koyudan açık tona. |
| MonochromaticPalette2 | `2` | accent2 tema rengi geçişi, koyudan açık tona. |
| MonochromaticPalette3 | `3` | accent3 tema rengi geçişi, koyudan açık tona. |
| MonochromaticPalette4 | `4` | accent4 tema rengi geçişi, koyudan açık tona. |
| MonochromaticPalette5 | `5` | accent5 tema rengi geçişi, koyudan açık tona. |
| MonochromaticPalette6 | `6` | accent6 tema rengi geçişi, koyudan açık tona. |
| MonochromaticPalette7 | `7` | accent7 tema rengi geçişi. |
| MonochromaticPalette8 | `8` | accent1 tema rengi geçişi, açıkdan koyuya. |
| MonochromaticPalette9 | `9` | accent2 tema rengi geçişi, açıkdan koyuya. |
| MonochromaticPalette10 | `10` | accent3 tema rengi geçişi, açıkdan koyuya. |
| MonochromaticPalette11 | `11` | accent4 tema rengi geçişi, açıkdan koyuya. |
| MonochromaticPalette12 | `12` | accent5 tema rengi geçişi, açıkdan koyuya. |
| MonochromaticPalette13 | `13` | accent6 tema rengi geçişi, açıkdan koyuya. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartColorPaletteTypeDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Renk paletini göstermek için bir örnek grafik ekle
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // Farklı ChartColorPaletteType enum değerlerini kullanarak göster
                ChartColorPaletteType palette1 = ChartColorPaletteType.MonochromaticPalette1;
                ChartColorPaletteType palette5 = ChartColorPaletteType.MonochromaticPalette5;
                ChartColorPaletteType palette8 = ChartColorPaletteType.MonochromaticPalette8;

                // Enum değerlerini görüntüle
                Console.WriteLine($"MonochromaticPalette1 value: {(int)palette1}");
                Console.WriteLine($"MonochromaticPalette5 value: {(int)palette5}");
                Console.WriteLine($"MonochromaticPalette8 value: {(int)palette8}");

                // Çalışma kitabını kaydedin
                workbook.Save("ChartColorPaletteTypeDemo.xlsx");
                Console.WriteLine("ChartColorPaletteType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ChartColorPaletteType: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


