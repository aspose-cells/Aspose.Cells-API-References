---
title: "Style.ShrinkToFit"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Rappresenta se il testo si riduce automaticamente per adattarsi alla larghezza della colonna disponibile"
type: docs
url: /it/net/aspose.cells/style/shrinktofit/
---
## Style.ShrinkToFit property

Rappresenta se il testo si riduce automaticamente per adattarsi alla larghezza della colonna disponibile.

```csharp
public bool ShrinkToFit { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // Crea un oggetto cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla collezione di celle
            Cells cells = worksheet.Cells;
            
            // Imposta del testo nella cella A1 più lungo della larghezza della colonna
            cells["A1"].PutValue("This is a long text that needs shrinking to fit");
            
            // Imposta la larghezza della colonna più piccola della lunghezza del testo
            cells.SetColumnWidth(0, 10);
            
            // Ottieni lo stile della cella A1
            Style style = cells["A1"].GetStyle();
            
            // Imposta ShrinkToFit su true
            style.ShrinkToFit = true;
            
            // Applica lo stile alla cella A1
            cells["A1"].SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("ShrinkToFitDemo.xlsx");
            
            Console.WriteLine("ShrinkToFit demo completed successfully.");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


