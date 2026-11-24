---
title: "Picture.OriginalWidthInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Eigenschaft. Gibt die ursprüngliche Breite des Bildes in Zoll zurück"
type: docs
url: /de/net/aspose.cells.drawing/picture/originalwidthinch/
---
## Picture.OriginalWidthInch property

Liest die ursprüngliche Breite des Bildes, in der Einheit Zoll.

```csharp
public double OriginalWidthInch { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge ein Bild hinzu (ersetze "example.jpg" durch deinen tatsächlichen Bildpfad)
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            // Erhalte und zeige die ursprüngliche Breite in Zoll an
            double picWidthInch = pic.OriginalWidthInch;
            Console.WriteLine($"Original picture width: {picWidthInch} inches");
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Siehe auch

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


