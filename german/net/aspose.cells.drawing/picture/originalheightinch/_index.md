---
title: "Picture.OriginalHeightInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Eigenschaft. Liefert die ursprüngliche Höhe des Bildes in Zoll"
type: docs
url: /de/net/aspose.cells.drawing/picture/originalheightinch/
---
## Picture.OriginalHeightInch property

Liest die ursprüngliche Höhe des Bildes, in der Einheit Zoll.

```csharp
public double OriginalHeightInch { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            Console.WriteLine("Original picture height in inches: " + pic.OriginalHeightInch);
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Siehe auch

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


