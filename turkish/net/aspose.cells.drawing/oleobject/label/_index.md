---
title: "OleObject.Label"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject özelliği. Bağlı ole nesnesinin görüntüleme etiketini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/label/
---
## OleObject.Label property

Bağlı ole nesnesinin görüntü etiketini alır ve ayarlar.

```csharp
public string Label { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyLabelDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Etiketli bir OLE nesnesi ekleyin
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.Label = "label_nameです";

            // Workbook'ı kaydet ve yeniden yükle
            string outputPath = "output.xlsx";
            workbook.Save(outputPath);
            
            // Etiket özelliğini doğrulayın
            Workbook loadedWorkbook = new Workbook(outputPath);
            OleObject loadedOleObject = loadedWorkbook.Worksheets[0].OleObjects[0];
            Console.WriteLine("OLE Object Label: " + loadedOleObject.Label);
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


