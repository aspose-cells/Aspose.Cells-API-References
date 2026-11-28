---
title: "MsoLineFormatHelper.DashStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoLineFormatHelper özelliği. Belirtilen satır için kesikli stilini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/msolineformathelper/dashstyle/
---
## MsoLineFormatHelper.DashStyle property

Belirtilen çizgi için kesikli stilini alır veya ayarlar.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyDashStyleDemo
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

                // Mevcut DashStyle değerini göster
                Console.WriteLine("Current DashStyle: " + lineFormat.DashStyle);

                // Yeni bir DashStyle değeri ayarla (çünkü okuma/yazma yapılabilir)
                lineFormat.DashStyle = MsoLineDashStyle.DashDot;
                Console.WriteLine("Updated DashStyle: " + lineFormat.DashStyle);

                // Özelliğin davranışı nasıl etkilediğini göster
                Console.WriteLine("Line dash style has been updated to: " + lineFormat.DashStyle);

                // Sonucu kaydet
                workbook.Save("DashStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line dash style.");
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

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


