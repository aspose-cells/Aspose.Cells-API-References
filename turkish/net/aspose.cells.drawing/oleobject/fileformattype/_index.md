---
title: "OleObject.FileFormatType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject özelliği. Gömülü ole nesnesi verisinin dosya türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/fileformattype/
---
## OleObject.FileFormatType property

Gömülü ole nesne verisinin dosya türünü alır ve ayarlar

```csharp
public FileFormatType FileFormatType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyFileFormatTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına (dosya verisi olmadan) bir OLE nesnesi ekleyin
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, null);
            
            // Eklenen OLE nesnesini alın
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            
            // Dosya formatı türünü ayarlayın ve gösterin
            oleObject.FileFormatType = FileFormatType.Docm;
            Console.WriteLine("OLE Object File Format Type: " + oleObject.FileFormatType);
            
            // Çalışma kitabını kaydedin
            workbook.Save("OleObjectFileFormatTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [FileFormatType](../../../aspose.cells/fileformattype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


