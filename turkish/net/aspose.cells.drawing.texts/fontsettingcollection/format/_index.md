---
title: "FontSettingCollection.Format"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSettingCollection yöntemi. Metni yazı tipi ayarıyla biçimlendirin"
type: docs
url: /tr/net/aspose.cells.drawing.texts/fontsettingcollection/format/
---
## FontSettingCollection.Format method

Metni font ayarıyla biçimlendir.

```csharp
public void Format(int startIndex, int length, Font font, StyleFlag flag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | Int32 | Başlangıç indeksi. |
| uzunluk | Int32 | Uzunluk. |
| yazı tipi | Yazı Tipi | Yazı tipi. |
| bayrak | StyleFlag | Yazı tipinin bayrakları. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodFormatWithInt32Int32FontStyleFlagDemo
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
            fontSettingCollection.Text = "Sample Text for Formatting";

            try
            {
                // Bir stil oluşturun ve yazı tipi özelliklerini ayarlayın
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                style.Font.IsBold = true;
                style.Font.Color = System.Drawing.Color.Red;

                // Uygulanacak yazı tipi özelliklerini belirtmek için stil bayrağı oluştur
                StyleFlag styleFlag = new StyleFlag();
                styleFlag.FontName = true;
                styleFlag.FontSize = true;
                styleFlag.FontBold = true;
                styleFlag.FontColor = true;

                // 7 ile 11. indeks arasındaki karakterleri biçimlendirin ("Text" kelimesi)
                fontSettingCollection.Format(7, 4, style.Font, styleFlag);

                // Etkisini göstermek için çalışma kitabını kaydedin
                workbook.Save("FontSettingCollectionFormatDemo.xlsx");
                Console.WriteLine("Format method executed successfully. Text 'Text' is now bold, red Arial 14pt.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Format method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


