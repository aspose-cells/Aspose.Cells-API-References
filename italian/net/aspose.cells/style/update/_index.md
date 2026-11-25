---
title: "Style.Update"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Style. Applica lo stile denominato agli stili delle celle che utilizzano questo stile denominato. Funziona come fare clic sul pulsante OK dopo aver terminato la modifica dello stile. Si applica solo agli stili denominati"
type: docs
url: /it/net/aspose.cells/style/update/
---
## Style.Update method

Applica lo stile denominato agli stili delle celle che utilizzano questo stile denominato. Funziona come fare clic sul pulsante "ok" dopo aver terminato la modifica dello stile. Si applica solo agli stili denominati.

```csharp
public void Update()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodUpdateDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea uno stile
            Style style = workbook.CreateStyle();
            style.Number = 3; // Set to Percent format
            
            // Applica lo stile alla cella A1
            worksheet.Cells["A1"].SetStyle(style);
            
            // Modifica lo stile
            style.Number = 4; // Change to Currency format
            
            // Aggiorna le modifiche allo stile
            style.Update();
            
            // Verifica che lo stile sia stato aggiornato
            Console.WriteLine("Cell A1 Number Format: " + worksheet.Cells["A1"].GetStyle().Number);
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


