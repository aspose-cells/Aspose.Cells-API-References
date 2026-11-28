---
title: "MsoLineFormat.Transparency"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoLineFormat özelliği. Belirtilen doldurmanın şeffaflık derecesini 0.0 opak'tan 1.0 şeffaf'a kadar bir değer olarak döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/msolineformat/transparency/
---
## MsoLineFormat.Transparency property

Belirtilen dolgunun şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar.

```csharp
public double Transparency { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir yay şekli ekle
            ArcShape arc = worksheet.Shapes.AddArc(1, 0, 1, 0, 100, 100);

            // Şeffaflık dahil olmak üzere satır biçim özelliklerini ayarla
            arc.LineFormat.ForeColor = System.Drawing.Color.Red;
            arc.LineFormat.Transparency = 0.5; // 50% transparent
            arc.LineFormat.Weight = 3;
            arc.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // Karşılaştırma için başka bir yay oluştur
            ArcShape arc2 = worksheet.Shapes.AddArc(1, 2, 1, 2, 100, 100);
            arc2.LineFormat.ForeColor = System.Drawing.Color.Red;
            arc2.LineFormat.Transparency = 0.5; // Same transparency
            arc2.LineFormat.Weight = 3;
            arc2.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // Şeffaflık özelliğini doğrula
            if (Math.Abs(arc.LineFormat.Transparency - arc2.LineFormat.Transparency) < 0.001)
            {
                Console.WriteLine("Transparency properties match: " + arc.LineFormat.Transparency);
            }
            else
            {
                Console.WriteLine("Transparency properties do not match");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("MsoLineFormatTransparencyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


