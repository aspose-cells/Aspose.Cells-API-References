---
title: "OleObject.AutoLoad"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject özelliği. Gömülü nesnenin ana çalışma kitabı açıldığında nesne verilerini otomatik olarak yüklemek için ana uygulamanın çağrılıp çağrılmayacağını belirtir."
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/autoload/
---
## OleObject.AutoLoad property

Ana çalışma kitabı açıldığında gömülü nesne için ana uygulamanın nesne verilerini otomatik olarak yüklemek üzere çağrılıp çağrılmayacağını belirtir.

```csharp
public bool AutoLoad { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoLoadDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir OleObject ekle
            int oleNumber = sheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            
            // OleObject özelliklerini ayarla
            OleObject ole = sheet.OleObjects[oleNumber];
            ole.ProgID = "Excel.Sheet";
            ole.ObjectData = new byte[0];
            
            // AutoLoad özelliğini göster
            ole.AutoLoad = true; // Automatically load the OleObject when the workbook opens
            
            // Çalışma kitabını kaydedin
            workbook.Save("OleObjectAutoLoadDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


