---
title: "FontSettingCollection.InsertText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSettingCollection yöntemi. Belirtilen konuma indeks ekler"
type: docs
url: /tr/net/aspose.cells.drawing.texts/fontsettingcollection/inserttext/
---
## FontSettingCollection.InsertText method

Pozisyonda indeks ekle.

```csharp
public void InsertText(int index, string text)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Başlangıç indeksi. |
| metin | String | Metin. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var fontSettingCollection = textBox.TextBody;

            // İlk metni ayarla
            fontSettingCollection.Text = "Initial Text";

            try
            {
                // Metni indeks 7'ye eklemek için InsertText yöntemini çağır
                fontSettingCollection.InsertText(7, " Inserted");

                // Değiştirilmiş metni göster
                Console.WriteLine("Text after insertion: " + fontSettingCollection.Text);
                
                // Çalışma kitabını kaydedin
                workbook.Save("FontSettingCollectionInsertTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertText method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


