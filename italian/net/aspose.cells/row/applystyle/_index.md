---
title: "Row.ApplyStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Row. Applica formati per un'intera riga"
type: docs
url: /it/net/aspose.cells/row/applystyle/
---
## Row.ApplyStyle method

Applica formati a un'intera riga.

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
    public class RowMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Imposta il contenuto HTML nella prima cella
            sheet.Cells[0, 0].HtmlString = @"<font style=""color: #49c131; font-weight: bold;"">Styled </font><font>text</font>";

            // Ottieni la prima riga e il suo stile
            Row row = sheet.Cells.Rows[0];
            Style style = row.GetStyle();
            
            // Modifica le proprietà dello stile
            style.IsTextWrapped = true;
            style.HorizontalAlignment = TextAlignmentType.Center;

            // Applica lo stile con flag specifici (solo l'andare a capo verrà applicato)
            row.ApplyStyle(style, new StyleFlag { WrapText = true });

            // Adattamento automatico per dimostrazione
            sheet.AutoFitRows();
            sheet.AutoFitColumns();

            // Salva la cartella di lavoro
            workbook.Save("RowApplyStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


