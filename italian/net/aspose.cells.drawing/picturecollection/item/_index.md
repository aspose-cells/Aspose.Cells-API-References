---
title: "PictureCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PictureCollection. Restituisce l'elemento Picture all'indice specificato"
type: docs
url: /it/net/aspose.cells.drawing/picturecollection/item/
---
## PictureCollection indexer

Restituisce l'elemento [`Picture`](../../picture/) all'indice specificato.

```csharp
public Picture this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni la collezione di immagini
            PictureCollection pictures = worksheet.Pictures;
            
            // Aggiungi un'immagine (sostituisci "image.png" con il percorso reale dell'immagine)
            int index = pictures.Add(1, 1, "image.png");
            
            // Accedi all'immagine usando la proprietà Item
            Picture pic = pictures[index];
            
            // Dimostra l'uso della proprietà Item
            Console.WriteLine($"Picture at index {index} has width: {pic.Width} and height: {pic.Height}");
            
            // Modifica le proprietà dell'immagine
            pic.Height = 200;
            pic.Width = 300;
            
            // Salva la cartella di lavoro
            workbook.Save("PictureCollectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../../picture/)
* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


