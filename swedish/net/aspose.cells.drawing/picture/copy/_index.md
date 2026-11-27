---
title: "Picture.Copy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-metod. Kopiera bilden"
type: docs
url: /sv/net/aspose.cells.drawing/picture/copy/
---
## Picture.Copy method

Kopiera bilden.

```csharp
public void Copy(Picture source, CopyOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | Bild | Källbilden. |
| alternativ | CopyOptions | Kopieringsalternativen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodCopyWithPictureCopyOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Infoga första bilden (med en exempelbildsökväg)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Infoga en andra bild (använd en exempelbildsökväg)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Kopiera bild 1 till bild 2 med CopyOptions
            CopyOptions options = new CopyOptions();
            pic2.Copy(pic1, options);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


