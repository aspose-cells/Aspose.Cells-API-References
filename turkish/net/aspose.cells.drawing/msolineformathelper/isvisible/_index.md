---
title: "MsoLineFormatHelper.IsVisible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoLineFormatHelper özelliği. Nesnenin görünür olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/msolineformathelper/isvisible/
---
## MsoLineFormatHelper.IsVisible property

Nesnenin görünür olup olmadığını gösterir.

```csharp
public bool IsVisible { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyIsVisibleDemo
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

                // Mevcut IsVisible değerini göster
                Console.WriteLine("Current IsVisible: " + lineFormat.IsVisible);

                // Yeni bir IsVisible değeri ayarla (çünkü okuma/yazma yapılabilir)
                lineFormat.IsVisible = false;
                Console.WriteLine("Updated IsVisible: " + lineFormat.IsVisible);

                // Özelliğin davranışı nasıl etkilediğini göster
                Console.WriteLine("Line visibility has been updated to: " + lineFormat.IsVisible);

                // Sonucu kaydet
                workbook.Save("IsVisibleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line visibility.");
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


