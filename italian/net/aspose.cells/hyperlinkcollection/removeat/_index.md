---
title: "HyperlinkCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo HyperlinkCollection. Rimuove il collegamento ipertestuale all'indice specificato in questa collezione"
type: docs
url: /it/net/aspose.cells/hyperlinkcollection/removeat/
---
## HyperlinkCollection.RemoveAt method

Rimuove il collegamento ipertestuale all'indice specificato in questa collezione.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice a base zero dell'elemento. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi un collegamento ipertestuale alla cella A1
            sheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Verifica che il collegamento ipertestuale esista prima della rimozione
            Console.WriteLine("Hyperlinks count before removal: " + sheet.Hyperlinks.Count);
            
            // Rimuove il collegamento ipertestuale all'indice 0
            sheet.Hyperlinks.RemoveAt(0);
            
            // Verifica che il collegamento ipertestuale sia stato rimosso
            Console.WriteLine("Hyperlinks count after removal: " + sheet.Hyperlinks.Count);
        }
    }
}
```

### Vedi anche

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


