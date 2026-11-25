---
title: "Class Column"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Column class. Rappresenta una singola colonna in un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/column/
---
## Column class

Rappresenta una singola colonna in un foglio di lavoro.

```csharp
public class Column
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [GroupLevel](../../aspose.cells/column/grouplevel/) { get; set; } | Ottiene il livello di gruppo della colonna. |
| [HasCustomStyle](../../aspose.cells/column/hascustomstyle/) { get; } | Indica se questa colonna ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dal workbook). |
| [Index](../../aspose.cells/column/index/) { get; } | Restituisce l'indice di questa colonna. |
| [IsCollapsed](../../aspose.cells/column/iscollapsed/) { get; set; } | se la colonna è compressa |
| [IsHidden](../../aspose.cells/column/ishidden/) { get; set; } | Indica se la colonna è nascosta. |
| [Style](../../aspose.cells/column/style/) { get; } | (**Obsoleto.**) Restituisce lo stile di questa colonna. |
| [Width](../../aspose.cells/column/width/) { get; set; } | Restituisce e imposta la larghezza della colonna in unità di caratteri. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ApplyStyle](../../aspose.cells/column/applystyle/)(Style, StyleFlag) | Applica formati a un'intera colonna. |
| [GetStyle](../../aspose.cells/column/getstyle/)() | Restituisce lo stile di questa colonna. |
| [SetStyle](../../aspose.cells/column/setstyle/)(Style) | Imposta lo stile di questa colonna. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnDemo
    {
        public static void ColumnExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Ottenere il riferimento del primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un nuovo Stile al Workbook
            Style style = workbook.CreateStyle();

            // Impostazione del colore di sfondo su Blu
            style.BackgroundColor = Color.Blue;

            // Impostazione del colore di primo piano su Rosso
            style.ForegroundColor = Color.Red;

            // Impostazione del modello di sfondo
            style.Pattern = BackgroundType.DiagonalStripe;

            // Nuovo flag di stile
            StyleFlag styleFlag = new StyleFlag();

            // Imposta tutti gli stili
            styleFlag.All = true;

            // Ottieni la prima colonna
            Column column = worksheet.Cells.Columns[0];

            // Applica lo stile alla prima colonna
            column.ApplyStyle(style, styleFlag);

            // Impostazione di proprietà aggiuntive
            column.Width = 20.0; // Setting the column width
            column.IsHidden = false; // Setting the column visibility
            column.IsCollapsed = false; // Setting the column collapsed state

            // Salvataggio del file Excel
            workbook.Save("ColumnExample.xlsx");
            workbook.Save("ColumnExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


