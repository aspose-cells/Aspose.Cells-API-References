---
title: "MsoLineFormatHelper.ForeColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoLineFormatHelper özelliği. Kenar çizgi ön rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/msolineformathelper/forecolor/
---
## MsoLineFormatHelper.ForeColor property

Kenarlık çizgi ön plan rengini alır ve ayarlar.

```csharp
public Color ForeColor { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyForeColorDemo
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

                // Mevcut ForeColor değerini gösterin
                Console.WriteLine("Current ForeColor: " + lineFormat.ForeColor);

                // Yeni bir ForeColor ayarlayın (okunabilir/yazılabilir olduğu için)
                lineFormat.ForeColor = Color.Red;
                Console.WriteLine("Updated ForeColor: " + lineFormat.ForeColor);

                // Özelliğin davranışı nasıl etkilediğini göster
                Console.WriteLine("Line fore color has been updated to: " + lineFormat.ForeColor);

                // Sonucu kaydet
                workbook.Save("ForeColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line fore color.");
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


