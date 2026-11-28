---
title: "TextOptions.Spacing"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextOptions özelliği. Metin akışı içinde karakterler arasındaki boşluğu belirler"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textoptions/spacing/
---
## TextOptions.Spacing property

Bir metin çalıştırması içinde karakterler arasındaki boşluğu belirtir.

```csharp
public double Spacing { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertySpacingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 0, 100, 200);
            textBox.Text = "Sample Text with Spacing";

            // Metin kutusunun metin seçeneklerini al
            TextOptions textOptions = textBox.TextOptions;

            // Mevcut boşluk değerini göster
            Console.WriteLine("Current Spacing value: " + textOptions.Spacing);

            // Yeni boşluk değerlerini ayarla ve etkilerini gör
            textOptions.Spacing = 2.0; // Increased spacing
            Console.WriteLine("Text with increased spacing (2.0)");

            // İlk boşlukla çalışma kitabını kaydet
            workbook.Save("TextSpacingDemo1.xlsx");

            // Boşluğu negatif değere değiştir (karakterler daha yakın)
            textOptions.Spacing = -1.0;
            Console.WriteLine("Text with decreased spacing (-1.0)");

            // İkinci boşlukla çalışma kitabını kaydet
            workbook.Save("TextSpacingDemo2.xlsx");

            // Varsayılan boşluğa sıfırla
            textOptions.Spacing = 0.0;
            Console.WriteLine("Text with default spacing (0.0)");

            // Varsayılan boşlukla çalışma kitabını kaydet
            workbook.Save("TextSpacingDemo3.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


