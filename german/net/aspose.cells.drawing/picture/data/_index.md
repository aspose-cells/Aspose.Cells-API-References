---
title: "Picture.Data"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Eigenschaft. Gibt die Daten des Bildes zurück"
type: docs
url: /de/net/aspose.cells.drawing/picture/data/
---
## Picture.Data property

Ermittelt die Daten des Bildes.

```csharp
public byte[] Data { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge das erste Bild ein
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "example1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Füge das zweite Bild ein
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "example2.jpeg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Demonstriere die Data-Eigenschaft, indem Bilddaten kopiert werden
            pic2.Data = pic1.Data;
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Siehe auch

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


