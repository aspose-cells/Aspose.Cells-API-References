---
title: "Column.ApplyStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Column. Applica formati per un'intera colonna"
type: docs
url: /it/net/aspose.cells/column/applystyle/
---
## Column.ApplyStyle method

Applica formati a un'intera colonna.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | Stile | L'oggetto stile che verrà applicato. |
| flag | StyleFlag | Flag che indicano le proprietà di formattazione applicate. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Imposta testo multilinea nella colonna 2
            sheet.Cells[0, 1].Value = "Line1\nLine2";
            sheet.Cells[1, 1].Value = "Text with\nmultiple lines";
            sheet.Cells[2, 1].Value = "Another\nmulti-line\ntext";

            // Crea stile con testo a capo abilitato
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // Applica lo stile solo alla proprietà testo a capo della colonna 2
            sheet.Cells.Columns[1].ApplyStyle(style, new StyleFlag() { WrapText = true });

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


