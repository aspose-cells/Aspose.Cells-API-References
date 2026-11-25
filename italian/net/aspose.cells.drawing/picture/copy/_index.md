---
title: "Picture.Copy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Picture. Copia l'immagine"
type: docs
url: /it/net/aspose.cells.drawing/picture/copy/
---
## Picture.Copy method

Copia l'immagine.

```csharp
public void Copy(Picture source, CopyOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | Immagine | L'immagine di origine. |
| opzioni | CopyOptions | Le opzioni di copia. |

### Esempi

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
            
            // Inserisci la prima immagine (usando un percorso di immagine di esempio)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Inserisci una seconda immagine (usando un percorso di immagine di esempio)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Copia l'immagine 1 nell'immagine 2 con CopyOptions
            CopyOptions options = new CopyOptions();
            pic2.Copy(pic1, options);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


