---
title: "Font.ScriptOffset"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Ottiene e imposta lo spostamento di script in unità percentuale"
type: docs
url: /it/net/aspose.cells/font/scriptoffset/
---
## Font.ScriptOffset property

Ottiene e imposta lo spostamento dello script, in unità di percentuale

```csharp
public double ScriptOffset { get; set; }
```

### Osservazioni

Solo per forme e grafici.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyScriptOffsetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella A1 e imposta il suo valore
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("ScriptOffset Demo");

            // Ottieni lo stile e il font della cella
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Imposta ScriptOffset per dimostrare l'effetto apice/indice
            font.ScriptOffset = 10; // Positive for superscript, negative for subscript
            font.IsSuperscript = true; // Enable superscript

            // Applica lo stile modificato nuovamente alla cella
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("FontScriptOffsetDemo.xlsx");

            // Verifica il valore di ScriptOffset
            Console.WriteLine("ScriptOffset value: " + font.ScriptOffset);
        }
    }
}
```

### Vedi anche

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


