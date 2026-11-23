---
title: "Picture.SignatureLine"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Picture. Obtient et définit la ligne de signature"
type: docs
url: /fr/net/aspose.cells.drawing/picture/signatureline/
---
## Picture.SignatureLine property

Obtient et définit la ligne de signature

```csharp
public SignatureLine SignatureLine { get; set; }
```

### Exemples

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

### Voir aussi

* class [SignatureLine](../../signatureline/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


