---
title: "OleObject.IsAutoSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject özelliği. True, OLE nesnesi etkinleştirildiğinde gömülü içeriğin anlık görüntüsü boyutuna göre nesnenin boyutunun otomatik olarak değişeceğini gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/isautosize/
---
## OleObject.IsAutoSize property

True, OLE nesnesi etkinleştirildiğinde gömülü içeriğin anlık görüntüsü boyutuna göre OLE nesnesinin boyutunun otomatik olarak değişeceğini gösterir.

```csharp
public bool IsAutoSize { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir OLE nesnesi ekle (dosya verisini bayt dizisi olarak kullanarak)
            byte[] oleData = System.IO.File.ReadAllBytes(@"C:\example\test.docx");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, oleData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];

            // IsAutoSize özelliğini ayarla ve göster
            oleObject.IsAutoSize = true;
            Console.WriteLine("OLE Object AutoSize initially: " + oleObject.IsAutoSize);

            // Özelliği değiştir
            oleObject.IsAutoSize = false;
            Console.WriteLine("OLE Object AutoSize after change: " + oleObject.IsAutoSize);

            // Çalışma kitabını kaydedin
            workbook.Save("OleObjectIsAutoSizeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


