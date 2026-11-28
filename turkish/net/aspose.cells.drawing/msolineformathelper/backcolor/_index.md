---
title: "MsoLineFormatHelper.BackColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoLineFormatHelper özelliği. Kenar çizgisinin arka plan rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/msolineformathelper/backcolor/
---
## MsoLineFormatHelper.BackColor property

Kenarlık çizgi arka plan rengini alır ve ayarlar.

```csharp
public Color BackColor { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyBackColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Örnek bir çalışma sayfası oluşturun
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bazı veriler ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Çizgi biçimlendirmesini göstermek için bir şekil oluşturun
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Çizgi biçimini alın
                MsoLineFormat lineFormat = shape.LineFormat;

                // Mevcut BackColor değerini göster
                Console.WriteLine("Current BackColor: " + lineFormat.BackColor);

                // Yeni bir BackColor değeri ayarla (çünkü okuma/yazma yapılabilir)
                lineFormat.BackColor = Color.LightBlue;
                Console.WriteLine("Updated BackColor: " + lineFormat.BackColor);

                // Özelliğin davranışı nasıl etkilediğini göster
                Console.WriteLine("Line back color has been updated to: " + lineFormat.BackColor);

                // Sonucu kaydet
                workbook.Save("BackColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line back color.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


