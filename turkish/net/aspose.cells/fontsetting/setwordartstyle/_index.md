---
title: "FontSetting.SetWordArtStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSetting yöntemi. Önceden tanımlı WordArt stilini ayarlar"
type: docs
url: /tr/net/aspose.cells/fontsetting/setwordartstyle/
---
## FontSetting.SetWordArtStyle method

Önceden ayarlanmış WordArt stilini ayarlar.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | PresetWordArtStyle | Önceden tanımlı WordArt stili. |

### Açıklamalar

Yalnızca şekil/grafik metni için.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FontSettingMethodSetWordArtStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine biraz metin ekleyin
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text for WordArt");

            // A1 hücresindeki metin için yazı tipi ayarı oluşturun
            FontSetting fontSetting = new FontSetting(0, cell.StringValue.Length, workbook.Worksheets);

            try
            {
                // Yazı tipi ayarına WordArt stilini uygulayın
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle3);

                Console.WriteLine("WordArt style applied successfully to the text.");
                
                // Çalışma kitabını kaydederek etkiyi gösterin
                worksheet.AutoFitColumn(0);
                worksheet.AutoFitRow(0);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("FontSettingMethodSetWordArtStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


