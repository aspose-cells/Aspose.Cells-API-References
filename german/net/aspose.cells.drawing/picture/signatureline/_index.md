---
title: "Picture.SignatureLine"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Eigenschaft. Liest und setzt die Signaturzeile"
type: docs
url: /de/net/aspose.cells.drawing/picture/signatureline/
---
## Picture.SignatureLine property

Ruft die Signaturzeile ab und legt sie fest

```csharp
public SignatureLine SignatureLine { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertySignatureLineDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, (string)null);
            Picture pic = worksheet.Pictures[imgIndex];
            
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "Simon";
            signatureLine.Title = "Development";
            signatureLine.Email = "simon@aspose.com";
            
            pic.SignatureLine = signatureLine;
            workbook.Save("result.xlsx");
        }
    }
}
```

### Siehe auch

* class [SignatureLine](../../signatureline/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


