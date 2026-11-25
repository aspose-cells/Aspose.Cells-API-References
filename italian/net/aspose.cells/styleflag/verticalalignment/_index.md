---
title: "StyleFlag.VerticalAlignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. L'impostazione di allineamento verticale verrà applicata"
type: docs
url: /it/net/aspose.cells/styleflag/verticalalignment/
---
## StyleFlag.VerticalAlignment property

L'impostazione di allineamento verticale sarà applicata.

```csharp
public bool VerticalAlignment { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea uno stile con allineamento verticale
            Style style = workbook.CreateStyle();
            style.VerticalAlignment = TextAlignmentType.Center;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.Font.Color = Color.Blue;

            // Crea un flag di stile per applicare solo l'allineamento verticale e il colore del carattere
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.VerticalAlignment = true;
            styleFlag.FontColor = true;

            // Applica lo stile alla prima riga con il flag di stile
            Row row = sheet.Cells.Rows[0];
            row.ApplyStyle(style, styleFlag);

            // Imposta del testo nelle celle per vedere l'effetto
            sheet.Cells["A1"].PutValue("Vertically Centered");
            sheet.Cells["B1"].PutValue("Blue Text");

            // Salva la cartella di lavoro
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


