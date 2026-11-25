---
title: "NameCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo NameCollection. Rimuove il nome all'indice specificato"
type: docs
url: /it/net/aspose.cells/namecollection/removeat/
---
## NameCollection.RemoveAt method

Rimuove il nome all'indice specifico.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | indice del Name da rimuovere. |

### Osservazioni

Assicurati che il nome non sia referenziato dalle altre formule prima di chiamare il metodo. E se il nome è referenziato, impostare Name.RefersTo a null è meglio.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;
            NameCollection names = worksheets.Names;

            // Aggiungi i nomi alla collezione
            int firstIndex = names.Add("FirstRange");
            names[firstIndex].RefersTo = "=Sheet1!$A$1:$A$5";
            
            int secondIndex = names.Add("SecondRange");
            names[secondIndex].RefersTo = "=Sheet1!$B$1:$B$5";

            // Rimuovi il nome per indice
            names.RemoveAt(firstIndex);

            // Verifica la rimozione controllando il conteggio
            Console.WriteLine($"Remaining names count: {names.Count}");

            workbook.Save("NameCollectionRemoveAtExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


