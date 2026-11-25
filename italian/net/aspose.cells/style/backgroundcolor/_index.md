---
title: "Style.BackgroundColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene o imposta il colore di sfondo di uno stile"
type: docs
url: /it/net/aspose.cells/style/backgroundcolor/
---
## Style.BackgroundColor property

Ottiene o imposta il colore di sfondo di uno stile.

```csharp
public Color BackgroundColor { get; set; }
```

### Osservazioni

Se desideri impostare il colore di una cella, utilizza la proprietà Style.ForegroundColor. Solo se il modello di stile della cella è diverso da nessuno o solido, questa proprietà avrà effetto.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un oggetto stile
            Style style = workbook.CreateStyle();
            
            // Imposta il colore di sfondo su giallo
            style.BackgroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Applica lo stile alla cella A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with yellow background");
            cell.SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


