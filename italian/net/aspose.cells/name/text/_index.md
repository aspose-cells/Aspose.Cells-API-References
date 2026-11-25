---
title: "Name.Text"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Name. Ottiene il testo del nome dell'oggetto"
type: docs
url: /it/net/aspose.cells/name/text/
---
## Name.Text property

Ottiene il testo del nome dell'oggetto.

```csharp
public string Text { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo denominato
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // Imposta e visualizza la proprietà Text
            namedRange.Text = "MyCustomName";
            Console.WriteLine("Named range text: " + namedRange.Text);
            
            // Salva la cartella di lavoro
            workbook.Save("NamedRangeExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


