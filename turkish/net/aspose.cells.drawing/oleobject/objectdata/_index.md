---
title: "OleObject.ObjectData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject özelliği. Gömülü ole nesnesi verisini bayt dizisi olarak temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/objectdata/
---
## OleObject.ObjectData property

Gömülü ole nesne verisini bayt dizisi olarak temsil eder.

```csharp
public byte[] ObjectData { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            var workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            var worksheet = workbook.Worksheets[0];
            
            // Örnek dosya yolları (ortamınızdaki gerçek yollarla değiştirin)
            string imagePath = "logo.jpg";
            string oleDataPath = "test.xls";

            // İlk görüntü verisiyle OLE nesnesi ekleyin
            int oleIndex = worksheet.OleObjects.Add(10, 10, 300, 200, File.ReadAllBytes(imagePath));
            
            // OLE nesnesinin verisini değiştirin
            worksheet.OleObjects[oleIndex].ObjectData = File.ReadAllBytes(oleDataPath);
            
            // Çalışma kitabını kaydedin
            workbook.Save("OleObjectDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("OLE object demo created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


