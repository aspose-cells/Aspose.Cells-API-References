---
title: "ShadowEffect.Color"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShadowEffect özelliği. Gölgenin rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shadoweffect/color/
---
## ShadowEffect.Color property

Gölgenin rengini alır ve ayarlar.

```csharp
public CellsColor Color { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShadowEffectPropertyColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Gölge etkisini göstermek için bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Şekilden gölge etkisini al
                ShadowEffect shadowEffect = shape.ShadowEffect;

                // Yeni bir CellsColor nesnesi oluştur
                CellsColor shadowColor = workbook.CreateCellsColor();

                // RGB değerlerini kullanarak rengi kırmızı olarak ayarla
                shadowColor.Color = Color.Red;

                // Rengi gölge etkisine uygula
                shadowEffect.Color = shadowColor;

                // Mevcut renk değerini göster
                Console.WriteLine("Shadow Color (RGB): " + shadowEffect.Color.Color.ToString());
                Console.WriteLine("Shadow Color (ARGB): " + shadowEffect.Color.Argb);

                // Etkiyi göstermek için çalışma kitabını kaydedin
                workbook.Save("ShadowEffectColorDemo.xlsx");

                // Rengin kaydedildiğini doğrulamak için çalışma kitabını yeniden yükle
                Workbook loadedWorkbook = new Workbook("ShadowEffectColorDemo.xlsx");
                ShadowEffect loadedShadowEffect = loadedWorkbook.Worksheets[0].Shapes[0].ShadowEffect;

                // Yüklenen renk değerini göster
                Console.WriteLine("Loaded Shadow Color (RGB): " + loadedShadowEffect.Color.Color.ToString());
                Console.WriteLine("Loaded Shadow Color (ARGB): " + loadedShadowEffect.Color.Argb);
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


