---
title: "OleObject.DisplayAsIcon"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject özelliği. Belirtilen nesne bir simge olarak gösteriliyorsa ve görüntü otomatik olarak değişmeyecekse doğru"
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/displayasicon/
---
## OleObject.DisplayAsIcon property

Belirtilen nesne bir simge olarak görüntüleniyorsa ve resim otomatik olarak değişmeyecekse true.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir OLE nesnesi (PDF) ekleyin
            byte[] pdfData = File.ReadAllBytes("example.pdf");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfData);
            
            // OLE nesnesini alın
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.ProgID = "AcroExch.Document.DC";
            
            // DisplayAsIcon özelliğini göster
            oleObject.DisplayAsIcon = true; // Show as icon
            // oleObject.DisplayAsIcon = false; // Mümkünse içeriği göster
            
            // Çalışma kitabını kaydedin
            workbook.Save("OleObjectDisplayAsIconDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


