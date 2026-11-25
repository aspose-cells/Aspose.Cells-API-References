---
title: "OleObjectCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObjectCollection. Ottiene l'elemento OleObject all'indice specificato"
type: docs
url: /it/net/aspose.cells.drawing/oleobjectcollection/item/
---
## OleObjectCollection indexer

Ottiene l'elemento [`OleObject`](../../oleobject/) all'indice specificato.

```csharp
public OleObject this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi dati immagine di esempio
            byte[] binaryImg = File.ReadAllBytes("image1.png");
            
            // Aggiungi oggetto OLE al primo foglio di lavoro
            int idxOle = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, binaryImg);
            
            // Accedi all'oggetto OLE usando la proprietà Item
            OleObject objOle = workbook.Worksheets[0].OleObjects[idxOle];
            
            // Imposta le proprietà dell'oggetto incorporato
            byte[] binaryXlsx = File.ReadAllBytes("example.xlsx");
            objOle.SetEmbeddedObject(false, binaryXlsx, "SampleFile.xlsx", true, "Excel.Sheet", false);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Verifica il file salvato
            Workbook savedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("OLE Object Source: " + savedWorkbook.Worksheets[0].OleObjects[0].ObjectSourceFullName);
        }
    }
}
```

### Vedi anche

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


