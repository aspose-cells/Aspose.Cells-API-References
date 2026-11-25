---
title: "Style.ForegroundArgbColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene e imposta il colore di primo piano con un valore ARGB a 32 bit"
type: docs
url: /it/net/aspose.cells/style/foregroundargbcolor/
---
## Style.ForegroundArgbColor property

Ottiene e imposta il colore di primo piano con un valore ARGB a 32 bit.

```csharp
public int ForegroundArgbColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundArgbColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea uno stile con un colore di primo piano specifico
            Style style = workbook.CreateStyle();
            style.ForegroundColor = System.Drawing.Color.FromArgb(255, 0, 255, 0); // Green color
            style.Pattern = BackgroundType.Solid;
            
            // Applica lo stile a una cella
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Ottieni e visualizza il valore del colore ARGB di primo piano
            int foregroundArgb = cell.GetStyle().ForegroundArgbColor;
            Console.WriteLine("Foreground ARGB Color: " + foregroundArgb);
            
            // Salva la cartella di lavoro
            workbook.Save("ForegroundColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


