---
title: "Class MsoLineFormatHelper"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.MsoLineFormatHelper class. Çizgi ve ok ucu biçimlendirmesini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/msolineformathelper/
---
## MsoLineFormatHelper class

Çizgi ve ok ucu biçimlendirmesini temsil eder.

```csharp
public class MsoLineFormatHelper
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformathelper/backcolor/) { get; set; } | Kenarlık çizgi arka plan rengini alır ve ayarlar. |
| [DashStyle](../../aspose.cells.drawing/msolineformathelper/dashstyle/) { get; set; } | Belirtilen çizgi için kesikli stilini alır veya ayarlar. |
| [ForeColor](../../aspose.cells.drawing/msolineformathelper/forecolor/) { get; set; } | Kenarlık çizgi ön plan rengini alır ve ayarlar. |
| [IsVisible](../../aspose.cells.drawing/msolineformathelper/isvisible/) { get; set; } | Nesnenin görünür olup olmadığını gösterir. |
| [Style](../../aspose.cells.drawing/msolineformathelper/style/) { get; set; } | Belirtilen aralığın stilini temsil eden bir Style nesnesi döndürür. |
| [Transparency](../../aspose.cells.drawing/msolineformathelper/transparency/) { get; set; } | Belirtilen dolgunun şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |
| [Weight](../../aspose.cells.drawing/msolineformathelper/weight/) { get; set; } | Çizginin kalınlığını puan (pt) biriminde döndürür veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassMsoLineFormatHelperDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Çizgi biçimlendirmesini göstermek için bir şekil oluşturun
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Şekilden doğrudan çizgi biçimini alın
                MsoLineFormat lineFormat = shape.LineFormat;

                // Çizgi biçimi üzerinde doğrudan özellikleri ayarlayın
                lineFormat.IsVisible = true;
                lineFormat.Style = MsoLineStyle.Single;
                lineFormat.ForeColor = Color.Blue;
                lineFormat.BackColor = Color.LightGray;
                lineFormat.DashStyle = MsoLineDashStyle.Solid;
                lineFormat.Transparency = 0.2;
                lineFormat.Weight = 2.5;

                // Yapılandırılmış özellikleri görüntüleyin
                Console.WriteLine($"Line is visible: {lineFormat.IsVisible}");
                Console.WriteLine($"Line style: {lineFormat.Style}");
                Console.WriteLine($"Fore color: {lineFormat.ForeColor}");
                Console.WriteLine($"Back color: {lineFormat.BackColor}");
                Console.WriteLine($"Dash style: {lineFormat.DashStyle}");
                Console.WriteLine($"Transparency: {lineFormat.Transparency}");
                Console.WriteLine($"Weight: {lineFormat.Weight}");

                // Çalışma kitabını kaydedin
                workbook.Save("MsoLineFormatHelperDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with MsoLineFormatHelper: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


