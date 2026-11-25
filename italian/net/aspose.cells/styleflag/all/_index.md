---
title: "StyleFlag.All"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verranno applicate tutte le proprietà"
type: docs
url: /it/net/aspose.cells/styleflag/all/
---
## StyleFlag.All property

Tutte le proprietà verranno applicate.

```csharp
public bool All { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyAllDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea uno stile con sfondo rosso solido
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;

            // Crea un flag di stile con la proprietà All impostata su true
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.All = true;

            // Applica lo stile alla prima colonna
            Column column = cells.Columns[0];
            column.ApplyStyle(style, styleFlag);

            // Verifica che lo stile sia stato applicato alle celle della colonna
            Cell cell = cells[0, 0];
            Style appliedStyle = cell.GetStyle();
            
            Console.WriteLine("Pattern: " + appliedStyle.Pattern);
            Console.WriteLine("Color: " + appliedStyle.ForegroundColor);
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


