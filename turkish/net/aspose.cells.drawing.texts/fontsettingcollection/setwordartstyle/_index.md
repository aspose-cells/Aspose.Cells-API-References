---
title: "FontSettingCollection.SetWordArtStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSettingCollection yöntemi. Önceden ayarlanmış WordArt stilini ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/fontsettingcollection/setwordartstyle/
---
## FontSettingCollection.SetWordArtStyle method

Önceden ayarlanmış WordArt stilini ayarlar.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | PresetWordArtStyle | Önceden tanımlı WordArt stili. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodSetWordArtStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // İlk metni ayarla
            fontSettingCollection.Text = "Sample Text for WordArt Styling";

            try
            {
                // WordArtStyle7 (Gradyan Doldurma - Mavi, Vurgu 1, Yansıma) ile SetWordArtStyle yöntemini çağır
                fontSettingCollection.SetWordArtStyle(PresetWordArtStyle.WordArtStyle7);

                Console.WriteLine("WordArt style applied successfully to the text box.");

                // Etkisini göstermek için çalışma kitabını kaydedin
                workbook.Save("FontSettingCollectionSetWordArtStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


