---
title: "Picture.IsSameSetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-metod. Returnerar om formen är densamma"
type: docs
url: /sv/net/aspose.cells.drawing/picture/issamesetting/
---
## Picture.IsSameSetting method

Returnerar om formen är densamma.

```csharp
public override bool IsSameSetting(object obj)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | Object |  |

### Exempel

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
            
            // Infoga första bilden (med en exempelbildsökväg)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Infoga andra bilden (med en annan exempelbildsökväg)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Jämför bilden med sig själv
            if (pic1.IsSameSetting(pic1))
            {
                Console.WriteLine("pic1 and pic1 are the same");
            }
            
            // Jämför olika bilder
            if (!pic1.IsSameSetting(pic2))
            {
                Console.WriteLine("pic1 and pic2 are different");
            }
        }
    }
}
```

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


