---
title: "FontSettingCollection.Replace"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSettingCollection yöntemi. Metni değiştir"
type: docs
url: /tr/net/aspose.cells.drawing.texts/fontsettingcollection/replace/
---
## Replace(int, int, string) {#replace}

Metni değiştir.

```csharp
public void Replace(int index, int count, string text)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Başlangıç indeksi. |
| sayım | Int32 | Karakter sayısı. |
| metin | String | Metin. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodReplaceWithInt32Int32StringDemo
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
            fontSettingCollection.Text = "Original text to be modified";

            try
            {
                // Replace yöntemini çağırarak 9. indeksten başlayarak 8 karakteri yeni metinle değiştirin
                fontSettingCollection.Replace(9, 8, "replaced");

                // Değiştirilmiş metni göster
                Console.WriteLine("Text after replacement: " + fontSettingCollection.Text);

                // Çalışma kitabını kaydedin
                workbook.Save("FontSettingCollectionReplaceDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string) {#replace_1}

Metni değiştir.

```csharp
public void Replace(string oldValue, string newValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| oldValue | String | Eski metin. |
| yeniDeğer | String | Yeni metin. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir şekil ekleyin ve metni ayarlayın
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample text ３４ for replacement";
            
            // Şekildeki metni değiştirin
            shape.TextBody.Replace("３４", "ABC");
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


