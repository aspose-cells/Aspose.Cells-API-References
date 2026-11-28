---
title: "Style.ForegroundArgbColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. 32 bit ARGB değeriyle ön plan rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/style/foregroundargbcolor/
---
## Style.ForegroundArgbColor property

32-bit ARGB değeriyle ön plan rengini alır ve ayarlar.

```csharp
public int ForegroundArgbColor { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundArgbColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Belirli bir ön plan rengiyle stil oluştur
            Style style = workbook.CreateStyle();
            style.ForegroundColor = System.Drawing.Color.FromArgb(255, 0, 255, 0); // Green color
            style.Pattern = BackgroundType.Solid;
            
            // Stili bir hücreye uygula
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Ön plan ARGB renk değerini al ve göster
            int foregroundArgb = cell.GetStyle().ForegroundArgbColor;
            Console.WriteLine("Foreground ARGB Color: " + foregroundArgb);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ForegroundColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


