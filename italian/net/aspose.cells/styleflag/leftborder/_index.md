---
title: "StyleFlag.LeftBorder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verranno applicate le impostazioni del bordo sinistro"
type: docs
url: /it/net/aspose.cells/styleflag/leftborder/
---
## StyleFlag.LeftBorder property

Le impostazioni del bordo sinistro saranno applicate.

```csharp
public bool LeftBorder { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLeftBorderDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];

            // Crea un intervallo e applica lo stile del bordo sinistro
            var range = worksheet.Cells.CreateRange(1, 1, 1, 1);
            range.PutValue("Left Border Demo", false, false);

            // Crea stile e flag
            var style = workbook.CreateStyle();
            var flag = new StyleFlag();

            // Imposta le proprietà del bordo sinistro
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thick;
            flag.LeftBorder = true;

            // Applica lo stile con il flag del bordo sinistro
            range.ApplyStyle(style, flag);

            // Verifica che il bordo sinistro sia stato applicato
            var appliedStyle = worksheet.Cells[1, 1].GetStyle();
            Console.WriteLine($"Left border color: {appliedStyle.Borders[BorderType.LeftBorder].Color}");
            Console.WriteLine($"Left border style: {appliedStyle.Borders[BorderType.LeftBorder].LineStyle}");

            // Salva la cartella di lavoro
            workbook.Save("LeftBorderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


