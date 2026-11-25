---
title: "OleObjectCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo OleObjectCollection. Rimuove l'elemento all'indice specificato"
type: docs
url: /it/net/aspose.cells.drawing/oleobjectcollection/removeat/
---
## OleObjectCollection.RemoveAt method

Rimuove l'elemento all'indice specificato.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice specificato. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi oggetti OLE di esempio (3 oggetti)
            for (int i = 0; i < 3; i++)
            {
                sheet.OleObjects.Add(i * 10, i * 10, 100, 100, new byte[0]);
            }

            Console.WriteLine("Before removal - OLE Objects count: " + sheet.OleObjects.Count);
            
            // Rimuovi gli oggetti OLE uno alla volta usando RemoveAt(int index)
            for (int i = sheet.OleObjects.Count - 1; i >= 0; i--)
            {
                sheet.OleObjects.RemoveAt(i);
            }

            Console.WriteLine("After removal - OLE Objects count: " + sheet.OleObjects.Count);
        }
    }
}
```

### Vedi anche

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


