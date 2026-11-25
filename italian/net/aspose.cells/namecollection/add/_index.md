---
title: "NameCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo NameCollection. Definisce un nuovo nome"
type: docs
url: /it/net/aspose.cells/namecollection/add/
---
## NameCollection.Add method

Definisce un nuovo nome.

```csharp
public int Add(string text)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | String | Il testo da usare come nome. |

### Valore di ritorno

[`Name`](../../name/) object index.

### Osservazioni

Il nome non può includere spazi e non può assomigliare a riferimenti di celle.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = wb.Worksheets[0];
            
            // Aggiungi un nome con riferimento a stringa
            int index = wb.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = wb.Worksheets.Names[index];
            
            // Imposta la formula a cui il nome fa riferimento
            namedRange.RefersTo = "=Sheet1!$A$1:$B$10";
            
            // Verifica e visualizza i risultati
            Console.WriteLine("Named Range RefersTo: " + namedRange.RefersTo);
            Console.WriteLine("Named Range Index: " + index);
            
            // Ottieni l'intervallo e mostra il suo indirizzo
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Range Address: " + range.Address);
        }
    }
}
```

### Vedi anche

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


