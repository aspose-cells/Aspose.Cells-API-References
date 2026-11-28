---
title: "OleObject.ImageSourceFullName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject özelliği. Bağlı görüntünün kaynak dosyasının yolunu ve adını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/imagesourcefullname/
---
## OleObject.ImageSourceFullName property

Bağlantılı görüntünün kaynak dosyasının yolunu ve adını alır veya ayarlar.

```csharp
public string ImageSourceFullName { get; set; }
```

### Açıklamalar

Varsayılan değer boş bir dizedir. SourceFullName boş bir dize değilse, görüntü bağlanır. SourceFullName boş bir dize değilse ancak Data null ise, görüntü bağlanır ve dosyada depolanmaz.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageSourceFullNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gömülmek üzere örnek PDF dosyası
            byte[] pdfBytes = File.ReadAllBytes("example.pdf");

            // Çalışma sayfasına bir OleObject ekle
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfBytes);
            OleObject oleObj = worksheet.OleObjects[oleIndex];

            // ImageSourceFullName dahil OleObject özelliklerini ayarlayın
            oleObj.DisplayAsIcon = false;
            oleObj.FileFormatType = FileFormatType.Pdf;
            oleObj.ImageSourceFullName = "sample_image.png"; // Demonstrating ImageSourceFullName usage
            oleObj.IsAutoSize = false;
            oleObj.IsLink = false;
            oleObj.ProgID = "Acrobat.Document.DC";

            // Çalışma kitabını kaydedin
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


