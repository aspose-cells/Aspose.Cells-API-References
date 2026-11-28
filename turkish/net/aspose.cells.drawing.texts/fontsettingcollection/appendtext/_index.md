---
title: "FontSettingCollection.AppendText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSettingCollection yöntemi. Metni ekler"
type: docs
url: /tr/net/aspose.cells.drawing.texts/fontsettingcollection/appendtext/
---
## FontSettingCollection.AppendText method

Metni ekler.

```csharp
public void AppendText(string text)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | String | Metin. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodAppendTextWithStringDemo
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
            fontSettingCollection.Text = "Hello, ";

            try
            {
                // Ek metin eklemek için AppendText yöntemini çağırın
                fontSettingCollection.AppendText("World!");

                // Değiştirilmiş metni göster
                Console.WriteLine("Text after append: " + fontSettingCollection.Text);

                // Çalışma kitabını kaydedin
                workbook.Save("FontSettingCollectionAppendTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AppendText method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


