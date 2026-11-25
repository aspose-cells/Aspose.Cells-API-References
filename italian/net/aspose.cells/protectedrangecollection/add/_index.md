---
title: "ProtectedRangeCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ProtectedRangeCollection. Aggiunge un elemento ProtectedRange alla collezione"
type: docs
url: /it/net/aspose.cells/protectedrangecollection/add/
---
## ProtectedRangeCollection.Add method

Aggiunge un elemento [`ProtectedRange`](../../protectedrange/) alla collezione.

```csharp
public int Add(string name, int startRow, int startColumn, int endRow, int endColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Titolo dell'intervallo. Questo è usato come descrittore, non come definizione di intervallo nominato. |
| startRow | Int32 | Indice della riga iniziale dell'intervallo. |
| startColumn | Int32 | Indice della colonna iniziale dell'intervallo. |
| endRow | Int32 | Indice della riga finale dell'intervallo. |
| endColumn | Int32 | Indice della colonna finale dell'intervallo. |

### Valore di ritorno

indice dell'oggetto.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeCollectionMethodAddWithStringInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ProtectedRangeCollection pranges = workbook.Worksheets[0].AllowEditRanges;
            
            // Aggiungi un intervallo protetto con nome e coordinate
            int index = pranges.Add("Range1", 0, 0, 10, 10);
            
            // Accedi all'intervallo aggiunto
            ProtectedRange range = pranges[index];
            
            // Imposta il descrittore di sicurezza
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            range.SecurityDescriptor = securityDescriptor;
            
            // Salva e verifica
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


