---
title: "Name.Comment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Name. Ottiene e imposta il commento del nome. Valida solo per Excel 2007 o versioni successive"
type: docs
url: /it/net/aspose.cells/name/comment/
---
## Name.Comment property

Ottiene e imposta il commento del nome. Si applica solo a Excel 2007 o versioni successive.

```csharp
public string Comment { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyCommentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un intervallo denominato con commento
            int index = workbook.Worksheets.Names.Add("TestRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            namedRange.Comment = "This is a test named range";
            
            // Salva la cartella di lavoro
            workbook.Save("NamedRangeWithComment.xlsx");
            
            // Carica la cartella di lavoro salvata per verificare il commento
            Workbook loadedWorkbook = new Workbook("NamedRangeWithComment.xlsx");
            Name loadedNamedRange = loadedWorkbook.Worksheets.Names[0];
            
            // Emetti il commento per dimostrare la funzionalità
            Console.WriteLine("Named Range Comment: " + loadedNamedRange.Comment);
        }
    }
}
```

### Vedi anche

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


