---
title: "StyleFlag.ShrinkToFit"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verrà applicata l'impostazione Riduci per adattare"
type: docs
url: /it/net/aspose.cells/styleflag/shrinktofit/
---
## StyleFlag.ShrinkToFit property

L'impostazione di riduzione per adattamento sarà applicata.

```csharp
public bool ShrinkToFit { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta dati di esempio in una cella
            cells["A1"].PutValue("This is a long text that needs to fit in the cell");
            
            // Crea uno stile con ShrinkToFit abilitato
            Style style = workbook.CreateStyle();
            style.ShrinkToFit = true;
            
            // Crea flag di stile e abilita il flag ShrinkToFit
            StyleFlag flag = new StyleFlag();
            flag.ShrinkToFit = true;
            
            // Applica lo stile all'intervallo di celle (usando esplicitamente Aspose.Cells.Range)
            Aspose.Cells.Range range = cells.CreateRange("A1");
            range.ApplyStyle(style, flag);
            
            // Imposta la larghezza della colonna per dimostrare il ridimensionamento
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // Salva la cartella di lavoro
            workbook.Save("ShrinkToFitDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


