---
title: "Worksheet.GridlineColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Worksheet property. Ottiene e imposta il colore della linea della griglia"
type: docs
url: /it/net/aspose.cells/worksheet/gridlinecolor/
---
## Worksheet.GridlineColor property

Ottiene e imposta il colore della griglia

```csharp
public Color GridlineColor { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il colore della linea della griglia su rosso
            worksheet.GridlineColor = Color.Red;
            
            // Salva la cartella di lavoro
            string outputPath = "GridlineColorDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Gridline color set to red and saved to: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


