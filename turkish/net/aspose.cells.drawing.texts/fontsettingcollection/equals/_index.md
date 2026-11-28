---
title: "FontSettingCollection.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSettingCollection yöntemi."
type: docs
url: /tr/net/aspose.cells.drawing.texts/fontsettingcollection/equals/
---
## FontSettingCollection.Equals method

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Biraz metin ayarlayın
            fontSettingCollection.Text = "Sample Text";

            try
            {
                // Karşılaştırma için başka bir FontSettingCollection oluşturun
                var anotherTextBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var anotherFontSettingCollection = anotherTextBox.TextBody;
                anotherFontSettingCollection.Text = "Sample Text";

                // İki koleksiyonu karşılaştırmak için Equals yöntemini çağırın
                bool areEqual = fontSettingCollection.Equals(anotherFontSettingCollection);

                // Sonucu göster
                Console.WriteLine($"Are the FontSettingCollections equal? {areEqual}");

                // Çalışma kitabını kaydedin
                workbook.Save("FontSettingCollectionEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Equals: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


