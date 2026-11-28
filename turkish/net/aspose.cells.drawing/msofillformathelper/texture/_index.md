---
title: "MsoFillFormatHelper.Texture"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFillFormatHelper özelliği. Doku doldurma tipini alır"
type: docs
url: /tr/net/aspose.cells.drawing/msofillformathelper/texture/
---
## MsoFillFormatHelper.Texture property

Doku dolgu tipini alır.

```csharp
public TextureType Texture { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Reflection;

    public class MsoFillFormatHelperPropertyTextureDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bir etiket ekle
            worksheet.Cells["A1"].Value = "Texture Property Demo";

            try
            {
                // Yansıma kullanarak MsoFillFormatHelper örneği oluştur (herkese açık yapıcı yok)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Texture özelliğinin mevcut değerini göster (yalnızca okunabilir)
                Console.WriteLine($"Current Texture type: {fillHelper.Texture}");

                // Özelliğin yalnızca okunabilir olduğunu, ayarlamaya çalışarak göster (yorum satırı olarak)
                // fillHelper.Texture = TextureType.Canvas; // Bu bir derleme hatasına neden olur

                // Referans için mevcut tüm doku tiplerini göster
                Console.WriteLine("\nAvailable Texture Types:");
                foreach (TextureType textureType in Enum.GetValues(typeof(TextureType)))
                {
                    Console.WriteLine($"- {textureType}");
                }

                // Başarılı yürütmeyi göstermek için çalışma kitabını kaydet.
                workbook.Save("TextureDemo.xlsx");

                Console.WriteLine("\nTexture property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Texture demo: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextureType](../../texturetype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


