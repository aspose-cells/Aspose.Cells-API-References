---
title: "ThemeColor.ThemeColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThemeColor yapıcı."
type: docs
url: /tr/net/aspose.cells/themecolor/themecolor/
---
## ThemeColor constructor

```csharp
public ThemeColor(ThemeColorType type, double tint)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | ThemeColorType | Tema tipi. |
| ton | Double | Renk tonu değeri. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorMethodCtorWithThemeColorTypeDoubleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // #ctor metodunu ThemeColorType ve Double parametreleriyle çağır
                ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // Tema rengini bir hücrenin stiline uygula
                Style style = workbook.CreateStyle();
                style.ForegroundThemeColor = themeColor;
                style.Pattern = BackgroundType.Solid;
                
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ThemeColor with Accent1 and 0.5 tint");
                cell.SetStyle(style);

                Console.WriteLine("ThemeColor constructor executed successfully with parameters (ThemeColorType.Accent1, 0.5)");
                Console.WriteLine($"ColorType: {themeColor.ColorType}, Tint: {themeColor.Tint}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ThemeColor constructor: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("ThemeColorCtorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


