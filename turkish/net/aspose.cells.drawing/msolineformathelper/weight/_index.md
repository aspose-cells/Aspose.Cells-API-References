---
title: "MsoLineFormatHelper.Weight"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoLineFormatHelper özelliği. Çizginin ağırlığını pt biriminde alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/msolineformathelper/weight/
---
## MsoLineFormatHelper.Weight property

Çizginin kalınlığını puan (pt) biriminde döndürür veya ayarlar.

```csharp
public double Weight { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyWeightDemo
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

                // Mevcut Weight değerini göster
                Console.WriteLine("Current Line Weight: " + lineFormat.Weight);

                // Yeni bir Weight değeri ayarla (çünkü okuma/yazma yapılabilir)
                lineFormat.Weight = 2.5;
                Console.WriteLine("Updated Line Weight: " + lineFormat.Weight);

                // Özelliğin davranışı nasıl etkilediğini göster
                Console.WriteLine("Line weight has been updated to: " + lineFormat.Weight);

                // Sonucu kaydet
                workbook.Save("WeightDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line weight.");
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


