---
title: "MsoFillFormatHelper.ForeColorTransparency"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFillFormatHelper özelliği. Belirtilen doldurmanın ön renk derecesini 0.0 opak'tan 1.0 şeffaf'a kadar bir değer olarak döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/msofillformathelper/forecolortransparency/
---
## MsoFillFormatHelper.ForeColorTransparency property

Belirtilen dolgunun ön renk derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar.

```csharp
public double ForeColorTransparency { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyForeColorTransparencyDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bir etiket ekle
            worksheet.Cells["A1"].Value = "ForeColorTransparency Demo";

            try
            {
                // Yansıma kullanarak MsoFillFormatHelper örneği oluştur (herkese açık yapıcı yok)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Varsayılan ForeColorTransparency değerini göster
                Console.WriteLine($"Default ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // Yeni bir ForeColor ve ForeColorTransparency ayarla
                fillHelper.ForeColor = Color.Blue;
                fillHelper.ForeColorTransparency = 0.5; // 50% transparency

                // Güncellenen değerleri göster
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");
                Console.WriteLine($"Updated ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // Şeffaflık değerini okumayı göster
                double transparency = fillHelper.ForeColorTransparency;
                Console.WriteLine($"Current transparency level: {transparency} (0.0=opaque, 1.0=clear)");

                // Başarılı yürütmeyi göstermek için çalışma kitabını kaydet.
                workbook.Save("ForeColorTransparencyDemo.xlsx");

                Console.WriteLine("ForeColorTransparency property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColorTransparency demo: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


