---
title: "OleObject.ProgID"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject özelliği. OLE nesnesinin ProgID'sini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/progid/
---
## OleObject.ProgID property

OLE nesnesinin ProgID'sini alır veya ayarlar.

```csharp
public string ProgID { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyProgIDDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir OLE nesnesi ekle
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0], "test.pdf");
            OleObject ole = worksheet.OleObjects[oleIndex];
            
            // OLE nesnesi için ProgID'yi ayarla
            ole.ProgID = "AcroExch.Document.DC";
            
            // ProgID'yi göster
            Console.WriteLine("OLE Object ProgID: " + ole.ProgID);

            // Çalışma kitabını kaydedin
            workbook.Save("OleObjectProgIDDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


