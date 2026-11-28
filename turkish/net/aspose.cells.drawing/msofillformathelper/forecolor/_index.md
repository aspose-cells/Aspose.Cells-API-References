---
title: "MsoFillFormatHelper.ForeColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFillFormatHelper özelliği. Doldurma ön renk alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/msofillformathelper/forecolor/
---
## MsoFillFormatHelper.ForeColor property

Doldurma ön rengini alır ve ayarlar.

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
    using System.Reflection;

    public class MsoFillFormatHelperPropertyForeColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bir etiket ekle
            worksheet.Cells["A1"].Value = "ForeColor Property Demo";

            try
            {
                // Yansıma kullanarak MsoFillFormatHelper örneği oluştur (herkese açık yapıcı yok)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Varsayılan ForeColor değerini göster
                Console.WriteLine($"Default ForeColor: {fillHelper.ForeColor}");

                // Yeni bir ForeColor değeri ayarla
                fillHelper.ForeColor = Color.FromArgb(255, 128, 0, 128); // Purple color
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");

                // ForeColor değerini almayı göster
                Color currentColor = fillHelper.ForeColor;
                Console.WriteLine($"Current ForeColor (RGB): R={currentColor.R}, G={currentColor.G}, B={currentColor.B}");

                // Başarılı yürütmeyi göstermek için çalışma kitabını kaydet.
                workbook.Save("ForeColorDemo.xlsx");

                Console.WriteLine("ForeColor property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColor demo: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


