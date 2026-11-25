---
title: "CellRichValue.Image"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellRichValue. Ottiene i dati immagine della cella"
type: docs
url: /it/net/aspose.cells/cellrichvalue/image/
---
## CellRichValue.Image property

Ottiene i dati dell'immagine della cella.

```csharp
public virtual byte[] Image { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class CellRichValuePropertyImageDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // Ottieni il valore ricco della cella che contiene l'immagine
            Cell cell = worksheet.Cells[0, 0];
            cell.PutValue("test data");
            cell.EmbeddedImage = picture.Data;

            // Accedi al valore ricco
            CellRichValue richValue = cell.GetRichValue();

            // Visualizza le proprietà dell'immagine
            Console.WriteLine("Image data length: " + (richValue.Image?.Length ?? 0));
            Console.WriteLine("Alt text: " + richValue.AltText);

            // Imposta nuovo testo alternativo per l'immagine
            richValue.AltText = "Sample product image";

            // Salva la cartella di lavoro
            workbook.Save("CellRichValueImageDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


