---
title: "Picture.Formula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Ottiene e imposta i dati della formula"
type: docs
url: /it/net/aspose.cells.drawing/picture/formula/
---
## Picture.Formula property

Ottiene e imposta i dati della formula.

```csharp
public string Formula { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Imposta la formula per l'immagine
            picture.Formula = "A1:A3";
            Console.WriteLine("Picture Formula: " + picture.Formula);

            // Modifica la formula
            picture.Formula = "B1:B3";
            Console.WriteLine("Updated Picture Formula: " + picture.Formula);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


