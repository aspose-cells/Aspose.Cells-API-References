---
title: "Picture.IsSameSetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Methode. Gibt zurück, ob die Form identisch ist"
type: docs
url: /de/net/aspose.cells.drawing/picture/issamesetting/
---
## Picture.IsSameSetting method

Gibt zurück, ob die Form gleich ist.

```csharp
public override bool IsSameSetting(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object |  |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodIsSameSettingWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge das erste Bild ein (unter Verwendung eines Beispielbildpfads)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Füge das zweite Bild ein (unter Verwendung eines anderen Beispielbildpfads)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Vergleiche das Bild mit sich selbst
            if (pic1.IsSameSetting(pic1))
            {
                Console.WriteLine("pic1 and pic1 are the same");
            }
            
            // Vergleiche verschiedene Bilder
            if (!pic1.IsSameSetting(pic2))
            {
                Console.WriteLine("pic1 and pic2 are different");
            }
        }
    }
}
```

### Siehe auch

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


