---
title: "Style.HorizontalAlignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene o imposta il tipo di allineamento orizzontale del testo in una cella"
type: docs
url: /it/net/aspose.cells/style/horizontalalignment/
---
## Style.HorizontalAlignment property

Ottiene o imposta il tipo di allineamento orizzontale del testo in una cella.

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta il testo nelle celle
            cells["A1"].PutValue("Left Aligned");
            cells["A2"].PutValue("Center Aligned");
            cells["A3"].PutValue("Right Aligned");

            // Ottieni gli oggetti stile
            Style styleLeft = cells["A1"].GetStyle();
            Style styleCenter = cells["A2"].GetStyle();
            Style styleRight = cells["A3"].GetStyle();

            // Imposta l'allineamento orizzontale
            styleLeft.HorizontalAlignment = TextAlignmentType.Left;
            styleCenter.HorizontalAlignment = TextAlignmentType.Center;
            styleRight.HorizontalAlignment = TextAlignmentType.Right;

            // Applica gli stili alle celle
            cells["A1"].SetStyle(styleLeft);
            cells["A2"].SetStyle(styleCenter);
            cells["A3"].SetStyle(styleRight);

            // Salva la cartella di lavoro
            workbook.Save("HorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


