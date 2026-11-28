---
title: "CellRichValue.Image"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellRichValue özelliği. Hücrenin görüntü verisini alır"
type: docs
url: /tr/net/aspose.cells/cellrichvalue/image/
---
## CellRichValue.Image property

Hücrenin görsel verisini alır.

```csharp
public virtual byte[] Image { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class CellRichValuePropertyImageDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir görüntü ekle
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // Görüntüyü içeren hücre zengin değerini al
            Cell cell = worksheet.Cells[0, 0];
            cell.PutValue("test data");
            cell.EmbeddedImage = picture.Data;

            // Zengin değere eriş
            CellRichValue richValue = cell.GetRichValue();

            // Görüntü özelliklerini göster
            Console.WriteLine("Image data length: " + (richValue.Image?.Length ?? 0));
            Console.WriteLine("Alt text: " + richValue.AltText);

            // Görüntü için yeni alternatif metni ayarla
            richValue.AltText = "Sample product image";

            // Çalışma kitabını kaydedin
            workbook.Save("CellRichValueImageDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


