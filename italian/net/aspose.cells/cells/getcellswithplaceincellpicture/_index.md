---
title: "Cells.GetCellsWithPlaceInCellPicture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene tutte le celle che contengono un'immagine incorporata"
type: docs
url: /it/net/aspose.cells/cells/getcellswithplaceincellpicture/
---
## Cells.GetCellsWithPlaceInCellPicture method

Restituisce tutte le celle che contengono un'immagine incorporata.

```csharp
public IEnumerator GetCellsWithPlaceInCellPicture()
```

### Valore di ritorno

Enumeratore per enumerare tutti gli oggetti Cell che contengono un'immagine incorporata

### Osservazioni

Se non vi è alcuna immagine impostata come "Place in Cell" in questo foglio di lavoro, verrà restituito null.

### Esempi

```csharp
using System;
using System.IO;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellsWithPlaceInCellPictureDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Aggiungi un'immagine al foglio di lavoro (questo non verrà conteggiato da GetCellsWithPlaceInCellPicture)
            workbook.Worksheets[0].Pictures.Add(0, 0, "sample.png");
            
            // Aggiungi un'immagine incorporata alla cella B3 (questo verrà conteggiato)
            workbook.Worksheets[0].Cells["B3"].EmbeddedImage = File.ReadAllBytes("sample.png");
            
            // Rimuovi l'immagine fluttuante
            workbook.Worksheets[0].Pictures.RemoveAt(0);

            // Ottieni le celle con immagini incorporate
            Cells cells = workbook.Worksheets[0].Cells;
            int count = 0;
            
            IEnumerator enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                    Console.WriteLine($"Found image in cell {cell.Name}");
                }
            }
            
            Console.WriteLine($"Total cells with embedded images: {count}");
            
            // Salva e ricarica per verificare la persistenza
            workbook.Save("output.xlsx");
            workbook = new Workbook("output.xlsx");
            
            // Verifica dopo il ricaricamento
            cells = workbook.Worksheets[0].Cells;
            count = 0;
            enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                }
            }
            Console.WriteLine($"After reload - cells with embedded images: {count}");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


