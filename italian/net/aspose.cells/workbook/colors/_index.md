---
title: "Workbook.Colors"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Workbook property. Restituisce i colori nella tavolozza per il foglio di calcolo"
type: docs
url: /it/net/aspose.cells/workbook/colors/
---
## Workbook.Colors property

Restituisce i colori nella tavolozza per il foglio di calcolo.

```csharp
public Color[] Colors { get; }
```

### Osservazioni

La tavolozza ha 56 voci, ciascuna rappresentata da un valore RGB.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyColorsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alla tavolozza dei colori predefinita
            Color[] colors = workbook.Colors;

            // Modifica alcuni colori nella tavolozza
            colors[0] = System.Drawing.Color.Red;      // Modify first color to Red
            colors[1] = System.Drawing.Color.Green;    // Modify second color to Green
            colors[2] = System.Drawing.Color.Blue;    // Modify third color to Blue

            // Crea un foglio di lavoro e aggiungi alcuni dati
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Color Demo");
            
            // Applica i colori modificati alle celle
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = colors[0];
            style1.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = colors[1];
            style2.Pattern = BackgroundType.Solid;
            worksheet.Cells["B2"].SetStyle(style2);
            
            Style style3 = workbook.CreateStyle();
            style3.ForegroundColor = colors[2];
            style3.Pattern = BackgroundType.Solid;
            worksheet.Cells["C2"].SetStyle(style3);

            // Salva la cartella di lavoro
            workbook.Save("WorkbookColorsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


