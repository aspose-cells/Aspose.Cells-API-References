---
title: "SignatureLine.Instructions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SignatureLine özelliği. İmzalama sırasında kullanıcıya gösterilen metni alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/signatureline/instructions/
---
## SignatureLine.Instructions property

İmzalama sırasında kullanıcıya gösterilen metni alır veya ayarlar.

```csharp
public string Instructions { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyInstructionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir imza satırı nesnesi oluştur
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Instructions = "Please sign here after reviewing the document.";

            // İmza satırını çalışma sayfasına (1,1) konumunda ekle
            worksheet.Shapes.AddSignatureLine(1, 1, signatureLine);

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


