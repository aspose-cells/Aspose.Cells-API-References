---
title: "Shape.GetRichFormattings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Metin içinde bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/shape/getrichformattings/
---
## Shape.GetRichFormattings method

Metin içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür.

```csharp
public FontSetting[] GetRichFormattings()
```

### Dönüş Değeri

Tüm Characters nesneleri

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zengin metinli bir şekil ekle (AddRectangle için doğru parametre sayısı)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is bold and this is italic";
            
            // Metnin bölümlerini biçimlendir
            shape.Characters(0, 4).Font.IsBold = true;
            shape.Characters(13, 6).Font.IsItalic = true;

            // Zengin metin biçimlendirmelerini al
            FontSetting[] formattings = shape.GetRichFormattings();

            // Biçimlendirme bilgilerini göster
            Console.WriteLine("Rich text formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"Text segment: '{shape.Text.Substring(setting.StartIndex, setting.Length)}'");
                Console.WriteLine($"Start index: {setting.StartIndex}");
                Console.WriteLine($"Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}");
                Console.WriteLine($"Italic: {setting.Font.IsItalic}");
                Console.WriteLine();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


