---
title: "SignatureLine.Title"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SignatureLine özelliği. Şarkıcının başlığını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/signatureline/title/
---
## SignatureLine.Title property

Şarkıcının unvanını alır veya ayarlar.

```csharp
public string Title { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyTitleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir imza satırı oluştur ve başlığını ayarla
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Title = "Development Lead";

            // İmza satırını çalışma sayfasının şekillerine konum parametreleriyle ekle
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Başlığı, özelliğin ayarlandığını göstermek için çıktı al
            Console.WriteLine("Signature Line Title: " + signatureLine.Title);
        }
    }
}
```

### Ayrıca Bakınız

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


