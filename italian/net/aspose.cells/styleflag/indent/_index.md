---
title: "StyleFlag.Indent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verrà applicata l'impostazione del livello di rientro"
type: docs
url: /it/net/aspose.cells/styleflag/indent/
---
## StyleFlag.Indent property

L'impostazione del livello di rientro sarà applicata.

```csharp
public bool Indent { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyIndentDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile con livello di rientro
            Style style = workbook.CreateStyle();
            style.IndentLevel = 2;
            style.HorizontalAlignment = TextAlignmentType.Left;

            // Crea flag di stile con la proprietà Indent impostata
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Indent = true;

            // Applica dati alle celle
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
                }
            }

            // Applica lo stile con rientro a un intervallo
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 5, 5);
            range.ApplyStyle(style, styleFlag);

            // Verifica che lo stile sia stato applicato
            Cell cell = worksheet.Cells["A1"];
            Style appliedStyle = cell.GetStyle();
            Console.WriteLine($"Indent Level: {appliedStyle.IndentLevel}");
            Console.WriteLine($"Alignment: {appliedStyle.HorizontalAlignment}");

            // Salva la cartella di lavoro
            workbook.Save("IndentStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


