---
title: "Picture.IsLink"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture property. Resim bir dosyaya bağlıysa doğru döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/picture/islink/
---
## Picture.IsLink property

Resim bir dosyaya bağlıysa true döndürür.

```csharp
public bool IsLink { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsLinkDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlantılı bir resim ekle
            int linkedPictureIndex = worksheet.Pictures.Add(0, 0, "https://example.com/image.jpg");
            Picture linkedPicture = worksheet.Pictures[linkedPictureIndex];

            // Gömülü bir resim ekle (örnek veri kullanarak)
            byte[] embeddedImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample image data
            using (MemoryStream stream = new MemoryStream(embeddedImageData))
            {
                int embeddedPictureIndex = worksheet.Pictures.Add(0, 5, stream);
                Picture embeddedPicture = worksheet.Pictures[embeddedPictureIndex];

                // IsLink özelliğini göster
                Console.WriteLine("Linked picture IsLink: " + linkedPicture.IsLink);
                Console.WriteLine("Embedded picture IsLink: " + embeddedPicture.IsLink);

                // IsLink'e göre farklı davranışı göster
                Console.WriteLine("\nLinked picture data is null: " + (linkedPicture.Data == null));
                Console.WriteLine("Embedded picture data length: " + embeddedPicture.Data.Length);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


