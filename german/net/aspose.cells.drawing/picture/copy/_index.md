---
title: "Picture.Copy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Methode. Kopiere das Bild"
type: docs
url: /de/net/aspose.cells.drawing/picture/copy/
---
## Picture.Copy method

Kopieren Sie das Bild.

```csharp
public void Copy(Picture source, CopyOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Bild | Das Quellbild. |
| Optionen | CopyOptions | Die Kopieroptionen. |

### Beispiele

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
            
            // Füge das erste Bild ein (unter Verwendung eines Beispielbildpfads)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Füge ein zweites Bild ein (unter Verwendung eines Beispielbildpfads)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Kopiere Bild 1 zu Bild 2 mit CopyOptions
            CopyOptions options = new CopyOptions();
            pic2.Copy(pic1, options);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


