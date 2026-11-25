---
title: "Style.IsGradient"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Indica se l'ombreggiatura della cella è un modello gradiente"
type: docs
url: /it/net/aspose.cells/style/isgradient/
---
## Style.IsGradient property

Indica se l'ombreggiatura della cella è un modello a gradiente.

```csharp
public bool IsGradient { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsGradientDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile
            Style style = workbook.CreateStyle();
            
            // Imposta lo sfondo gradiente
            style.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);
            
            // Applica lo stile a una cella
            worksheet.Cells["A1"].SetStyle(style);
            
            // Verifica se lo stile ha un gradiente
            bool isGradient = worksheet.Cells["A1"].GetStyle().IsGradient;
            
            // Restituisci il risultato
            Console.WriteLine("Cell A1 style has gradient: " + isGradient);
            
            // Salva la cartella di lavoro
            workbook.Save("GradientStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


