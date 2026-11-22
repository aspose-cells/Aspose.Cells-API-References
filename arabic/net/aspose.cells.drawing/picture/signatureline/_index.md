---
title: "Picture.SignatureLine"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Picture. تحصل وتضبط خط التوقيع"
type: docs
url: /ar/net/aspose.cells.drawing/picture/signatureline/
---
## Picture.SignatureLine property

يحصل على سطر التوقيع ويضبطه

```csharp
public SignatureLine SignatureLine { get; set; }
```

### أمثلة

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

### انظر أيضًا

* class [SignatureLine](../../signatureline/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


