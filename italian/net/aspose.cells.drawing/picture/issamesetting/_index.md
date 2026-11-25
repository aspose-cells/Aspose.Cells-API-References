---
title: "Picture.IsSameSetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Picture method. Restituisce se la forma è la stessa"
type: docs
url: /it/net/aspose.cells.drawing/picture/issamesetting/
---
## Picture.IsSameSetting method

Restituisce se la forma è la stessa.

```csharp
public override bool IsSameSetting(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object |  |

### Esempi

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
            
            // Inserisci la prima immagine (usando un percorso di immagine di esempio)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Inserisci la seconda immagine (usando un percorso di immagine di esempio diverso)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Confronta l'immagine con se stessa
            if (pic1.IsSameSetting(pic1))
            {
                Console.WriteLine("pic1 and pic1 are the same");
            }
            
            // Confronta immagini diverse
            if (!pic1.IsSameSetting(pic2))
            {
                Console.WriteLine("pic1 and pic2 are different");
            }
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


