---
title: "Picture.SourceFullName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture özelliği. Bağlantılı görüntünün kaynak dosyasının yolunu ve adını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/picture/sourcefullname/
---
## Picture.SourceFullName property

Bağlantılı görüntünün kaynak dosyasının yolunu ve adını alır veya ayarlar.

```csharp
public string SourceFullName { get; set; }
```

### Açıklamalar

Varsayılan değer boş bir dizedir. SourceFullName boş bir dize değilse, görüntü bağlanır. SourceFullName boş bir dize değilse ancak Data null ise, görüntü bağlanır ve dosyada depolanmaz.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertySourceFullNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bağlantılı bir resim ekle
            string imagePath = "example.png";
            Picture picture = worksheet.Shapes.AddLinkedPicture(0, 0, 100, 100, imagePath);

            // SourceFullName özelliğini göster
            Console.WriteLine("Picture SourceFullName: " + picture.SourceFullName);
            Console.WriteLine("Is linked picture: " + picture.IsLink);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


