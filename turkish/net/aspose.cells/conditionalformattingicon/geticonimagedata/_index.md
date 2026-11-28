---
title: "ConditionalFormattingIcon.GetIconImageData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConditionalFormattingIcon yöntemi. Simge seti verilerini alın"
type: docs
url: /tr/net/aspose.cells/conditionalformattingicon/geticonimagedata/
---
## ConditionalFormattingIcon.GetIconImageData method

İkon seti verisini al

```csharp
public static byte[] GetIconImageData(IconSetType type, int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | IconSetType | simgenin türü |
| indeks | Int32 | simgenin indeksi |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class ConditionalFormattingIconMethodGetIconImageDataWithIconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // GetIconImageData statik olduğu için örnek oluşturmanıza gerek yok
            
            try
            {
                // GetIconImageData'yı IconSetType.Arrows3 ve indeks 0 ile çağırın
                byte[] imageData = ConditionalFormattingIcon.GetIconImageData(IconSetType.Arrows3, 0);
                
                Console.WriteLine("Method executed successfully. Image data length: " + imageData.Length);
                
                // Görsel verisini gösterim için bir dosyaya kaydedin
                File.WriteAllBytes("icon_image.png", imageData);
                Console.WriteLine("Icon image saved to icon_image.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetIconImageData method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("ConditionalFormattingIconGetIconImageDataDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


