---
title: "Worksheet.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene o imposta il nome del foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/name/
---
## Worksheet.Name property

Ottiene o imposta il nome del foglio di lavoro.

```csharp
public string Name { get; set; }
```

### Osservazioni

La lunghezza massima del nome del foglio è 31. E non è possibile assegnare lo stesso nome (senza distinzione tra maiuscole e minuscole) a due fogli di lavoro. Ad esempio, non è possibile impostare "SheetName1" sul primo foglio di lavoro e impostare "SHEETNAME1" sul secondo foglio di lavoro.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e imposta il suo nome
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Aggiungi un nuovo foglio di lavoro con un nome specifico
            Worksheet newSheet = workbook.Worksheets.Add("ReportSheet");
            
            // Stampa i nomi di tutti i fogli di lavoro
            Console.WriteLine("Worksheet Names:");
            foreach (Worksheet ws in workbook.Worksheets)
            {
                Console.WriteLine(ws.Name);
            }
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetNamesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


