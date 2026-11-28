---
title: "SignatureLine.Signer"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SignatureLine özelliği. İmzayı alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/signatureline/signer/
---
## SignatureLine.Signer property

İmzayı yapanı alır veya ayarlar.

```csharp
public string Signer { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertySignerDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir imza satırı oluştur ve özelliklerini ayarla
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";

            // İmza satırını çalışma sayfasına 1. satır, 1. sütunda ekle
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Çalışma kitabını kaydedin
            workbook.Save("SignatureLineDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


