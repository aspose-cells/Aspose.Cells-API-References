---
title: "ShapeCollection.AddLinkedPicture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un'immagine collegata"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addlinkedpicture/
---
## ShapeCollection.AddLinkedPicture method

Aggiungi un'immagine collegata.

```csharp
public Picture AddLinkedPicture(int topRow, int leftColumn, int height, int width, 
    string sourceFullName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| altezza | Int32 | L'altezza della forma. In unità di pixel |
| larghezza | Int32 | La larghezza della forma. In unità di pixel |
| sourceFullName | String | Il percorso e il nome del file sorgente per l'immagine collegata |

### Valore di ritorno

[`Picture`](../../picture/) Picture object.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLinkedPictureWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi testo di esempio alla cella A1
            worksheet.Cells["A1"].PutValue("Image will be linked below:");
            
            // Aggiungi immagine collegata al foglio di lavoro
            string imageUrl = "https://example.com/sample.jpg";
            worksheet.Shapes.AddLinkedPicture(1, 1, 100, 100, imageUrl);
            
            // Salva la cartella di lavoro
            workbook.Save("output_with_linked_picture.xlsx");
            
            Console.WriteLine("Workbook saved with linked picture.");
        }
    }
}
```

### Vedi anche

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


