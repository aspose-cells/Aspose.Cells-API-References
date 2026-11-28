---
title: "TextOptions.UnderlineColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextOptions özelliği. Alt çizgi rengini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textoptions/underlinecolor/
---
## TextOptions.UnderlineColor property

Alt çizginin rengini alır veya ayarlar.

```csharp
public CellsColor UnderlineColor { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyUnderlineColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Metin seçeneklerini göstermek için metin içeren bir şekil ekle
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Underline Color Demo";
            
            // Şekilden TextOptions'ı al
            TextOptions textOptions = shape.TextOptions;

            try
            {
                // Mevcut UnderlineColor değerini göster
                CellsColor currentColor = textOptions.UnderlineColor;
                Console.WriteLine($"Current UnderlineColor - Type: {currentColor.Type}, Color: {currentColor.Color}");

                // Yeni bir UnderlineColor ayarla (özellik okuma-yazma olduğu için)
                CellsColor newColor = textOptions.UnderlineColor; // Use existing color object
                newColor.Color = System.Drawing.Color.Red;
                textOptions.UnderlineColor = newColor;

                // Etkiyi görmek için alt çizgiyi etkinleştir
                textOptions.Underline = FontUnderlineType.Single;

                // Yeni UnderlineColor değerini göster
                Console.WriteLine($"New UnderlineColor - Type: {textOptions.UnderlineColor.Type}, Color: {textOptions.UnderlineColor.Color}");

                // Etkiyi görmek için çalışma kitabını kaydet
                workbook.Save("UnderlineColorDemo.xlsx");
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
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


