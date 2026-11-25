---
title: "Cell.InsertText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Inserisce alcuni caratteri nella cella. Se la cella è formattata in modo ricco, questo metodo può mantenere la formattazione originale."
type: docs
url: /it/net/aspose.cells/cell/inserttext/
---
## Cell.InsertText method

Inserisce alcuni caratteri nella cella. Se la cella è formattata in rich text, questo metodo può mantenere la formattazione originale.

```csharp
public void InsertText(int index, string text)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice. |
| testo | String | Testo inserito. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla cella B3 e imposta il valore iniziale
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("OriginalText");
            
            // Inserisci testo nella posizione 6
            cell.InsertText(6, "Inserted");
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


