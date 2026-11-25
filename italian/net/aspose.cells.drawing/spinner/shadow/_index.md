---
title: "Spinner.Shadow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Spinner. Indica se la forma ha ombreggiatura 3D"
type: docs
url: /it/net/aspose.cells.drawing/spinner/shadow/
---
## Spinner.Shadow property

Indica se la forma ha ombreggiatura 3-D.

```csharp
public bool Shadow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyShadowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi uno spinner al foglio di lavoro
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);

            // Imposta le proprietà del spinner
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 50;

            // Dimostra la proprietà Shadow
            spinner.Shadow = true; // Enable 3D shadow effect
            Console.WriteLine("Spinner shadow enabled: " + spinner.Shadow);

            // Salva la cartella di lavoro
            workbook.Save("SpinnerShadowDemo.xlsx");

            // Carica la cartella di lavoro salvata per verificare la proprietà shadow
            Workbook verifyWorkbook = new Workbook("SpinnerShadowDemo.xlsx");
            Spinner verifySpinner = (Spinner)verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("Verified spinner shadow: " + verifySpinner.Shadow);
        }
    }
}
```

### Vedi anche

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


