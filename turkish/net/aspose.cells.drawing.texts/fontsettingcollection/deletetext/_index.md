---
title: "FontSettingCollection.DeleteText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSettingCollection yöntemi. Bazı karakterleri sil"
type: docs
url: /tr/net/aspose.cells.drawing.texts/fontsettingcollection/deletetext/
---
## FontSettingCollection.DeleteText method

Bazı karakterleri sil.

```csharp
public void DeleteText(int index, int count)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Başlangıç indeksi. |
| sayım | Int32 | Karakter sayısı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodDeleteTextWithInt32Int32Demo
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
            fontSettingCollection.Text = "This is sample text to demonstrate DeleteText method";

            try
            {
                // Orijinal metni göster
                Console.WriteLine("Original text: " + fontSettingCollection.Text);

                // DeleteText yöntemini çağırarak 5. indeksten başlayarak 7 karakteri kaldırın
                fontSettingCollection.DeleteText(5, 7);

                // Değiştirilmiş metni göster
                Console.WriteLine("Text after deletion: " + fontSettingCollection.Text);

                // Çalışma kitabını kaydedin
                workbook.Save("FontSettingCollectionDeleteTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DeleteText method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


