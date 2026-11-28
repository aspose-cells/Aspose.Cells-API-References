---
title: "OleObject.ImageData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject özelliği. Ole nesnesinin görüntüsünü bayt dizisi olarak temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/imagedata/
---
## OleObject.ImageData property

Ole nesnesinin görüntüsünü bayt dizisi olarak temsil eder.

```csharp
public byte[] ImageData { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Görüntü dosyasını bayt dizisine oku
            byte[] imageBytes = File.ReadAllBytes("image1.png");
            
            // Görüntü verisiyle OLE nesnesi ekle
            int oleIndex = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, imageBytes);
            OleObject oleObject = workbook.Worksheets[0].OleObjects[oleIndex];
            
            // Gömülü nesne özelliklerini ayarla
            oleObject.SetEmbeddedObject(false, imageBytes, "image1.png", true, "Sample Image", false);
            
            // ImageData özelliğinin kullanımını göster
            Console.WriteLine($"Image data length: {oleObject.ImageData.Length}");
            Console.WriteLine($"First byte: {oleObject.ImageData[0]}");
            Console.WriteLine($"Middle byte: {oleObject.ImageData[oleObject.ImageData.Length/2]}");
            Console.WriteLine($"Last byte: {oleObject.ImageData[oleObject.ImageData.Length-1]}");
            
            // Çalışma kitabını kaydedin
            workbook.Save("OleObjectWithImage.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


