---
title: "Border.ArgbColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Border. Ottiene e imposta il colore con un valore ARGB a 32 bit"
type: docs
url: /it/net/aspose.cells/border/argbcolor/
---
## Border.ArgbColor property

Ottiene e imposta il colore con un valore ARGB a 32 bit.

```csharp
public int ArgbColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyArgbColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella B2 e imposta un valore
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Border ARGB Color Demo");

            // Ottieni lo stile e i bordi
            Style style = cell.GetStyle();
            Border border = style.Borders[BorderType.TopBorder];

            // Imposta le proprietà del bordo includendo il colore ARGB
            border.LineStyle = CellBorderType.Thick;
            unchecked
            {
                border.ArgbColor = (int)0xFFFF0000; // Red color in ARGB format with unchecked cast
            }

            // Applica lo stile modificato alla cella
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("BorderArgbColorDemo.xlsx");

            // Verifica che il colore ARGB sia stato impostato correttamente
            Border savedBorder = workbook.Worksheets[0].Cells["B2"].GetStyle().Borders[BorderType.TopBorder];
            Console.WriteLine("ARGB Color of top border: " + savedBorder.ArgbColor.ToString("X8"));
        }
    }
}
```

### Vedi anche

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


