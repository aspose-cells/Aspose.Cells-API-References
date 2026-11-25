---
title: "WorksheetCollection.Names"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorksheetCollection proprietà. Restituisce la raccolta di tutti gli oggetti Name nel foglio di calcolo"
type: docs
url: /it/net/aspose.cells/worksheetcollection/names/
---
## WorksheetCollection.Names property

Ottiene la collezione di tutti gli oggetti Name nel foglio elettronico.

```csharp
public NameCollection Names { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyNamesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro con caratteri speciali nel nome
            Worksheet worksheet = workbook.Worksheets.Add("My.Test");
            
            // Accedi alla raccolta Names
            NameCollection names = workbook.Worksheets.Names;
            
            // Aggiungi un nuovo intervallo denominato
            int index = names.Add("My.Test!TestName");
            Name namedRange = names[index];
            
            // Imposta il riferimento dell'intervallo e dimostra l'uso
            namedRange.RefersTo = "=My.Test!$A$1:$B$2";
            
            // Restituisci le proprietà dell'intervallo denominato
            Console.WriteLine("Name: " + namedRange.Text);
            Console.WriteLine("FullText: " + namedRange.FullText);
            Console.WriteLine("RefersTo: " + namedRange.RefersTo);
        }
    }
}
```

### Vedi anche

* class [NameCollection](../../namecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


