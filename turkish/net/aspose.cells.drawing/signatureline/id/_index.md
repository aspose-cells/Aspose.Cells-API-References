---
title: "SignatureLine.Id"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SignatureLine özelliği. Bu imza satırı için tanımlayıcıyı alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/signatureline/id/
---
## SignatureLine.Id property

Bu imza satırı için tanımlayıcıyı alır veya ayarlar.

```csharp
public Guid Id { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir imza satırı nesnesi oluştur
            SignatureLine signatureLine = new SignatureLine();
            Guid signatureId = Guid.NewGuid();
            signatureLine.Id = signatureId;
            
            // İmza satırını çalışma sayfasına (1,1) konumunda ekle
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // İmza satırının kimliğini göster
            Console.WriteLine("Signature Line ID: " + signatureLine.Id);
        }
    }
}
```

### Ayrıca Bakınız

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


