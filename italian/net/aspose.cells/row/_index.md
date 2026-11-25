---
title: "Classe Row"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Row. Rappresenta una singola riga in un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/row/
---
## Row class

Rappresenta una singola riga in un foglio di lavoro.

```csharp
public class Row : IEnumerable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FirstCell](../../aspose.cells/row/firstcell/) { get; } | Ottiene il primo oggetto cella nella riga. |
| [FirstDataCell](../../aspose.cells/row/firstdatacell/) { get; } | Ottiene la prima cella non vuota nella riga. |
| [GroupLevel](../../aspose.cells/row/grouplevel/) { get; set; } | Ottiene il livello di gruppo della riga. |
| [HasCustomStyle](../../aspose.cells/row/hascustomstyle/) { get; } | Indica se questa riga ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dalla cartella di lavoro). |
| [Height](../../aspose.cells/row/height/) { get; set; } | Ottiene e imposta l'altezza della riga in unità di punti. |
| [Index](../../aspose.cells/row/index/) { get; } | Ottiene l'indice di questa riga. |
| [IsBlank](../../aspose.cells/row/isblank/) { get; } | Indica se la riga contiene dati |
| [IsCollapsed](../../aspose.cells/row/iscollapsed/) { get; set; } | se la riga è compressa |
| [IsHeightMatched](../../aspose.cells/row/isheightmatched/) { get; set; } | Indica se l'altezza della riga corrisponde all'impostazione corrente del carattere predefinito della cartella di lavoro. Il valore true di questa proprietà indica anche che l'altezza della riga è "automatica" senza un valore di altezza personalizzato impostato dall'utente. |
| [IsHidden](../../aspose.cells/row/ishidden/) { get; set; } | Indica se la riga è nascosta. |
| [Item](../../aspose.cells/row/item/) { get; } | Ottiene la cella. |
| [LastCell](../../aspose.cells/row/lastcell/) { get; } | Ottiene l'ultimo oggetto cella nella riga. |
| [LastDataCell](../../aspose.cells/row/lastdatacell/) { get; } | Ottiene l'ultima cella non vuota nella riga. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ApplyStyle](../../aspose.cells/row/applystyle/)(Style, StyleFlag) | Applica formati a un'intera riga. |
| [CopySettings](../../aspose.cells/row/copysettings/)(Row, bool) | Copia le impostazioni della riga, come stile, altezza, visibilità, ...ecc. |
| override [Equals](../../aspose.cells/row/equals/#equals_1)(object) | Verifica se questo oggetto si riferisce alla stessa riga di un altro. |
| [Equals](../../aspose.cells/row/equals/#equals)(Row) | Verifica se questo oggetto si riferisce alla stessa riga di un altro oggetto riga. |
| [GetCellByIndex](../../aspose.cells/row/getcellbyindex/)(int) | Ottieni la cella tramite indice specifico nella collezione di celle di questa riga. |
| [GetCellOrNull](../../aspose.cells/row/getcellornull/)(int) | Ottiene la cella o null nell'indice specifico. |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator)() | Ottiene l'enumeratore delle celle |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator_1)(bool, bool) | Ottiene un enumeratore che itera le celle attraverso questa riga. |
| [GetStyle](../../aspose.cells/row/getstyle/)() | Ottiene lo stile di questa riga. |
| [SetStyle](../../aspose.cells/row/setstyle/)(Style) | Imposta lo stile di questa riga. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;
    using System.Collections;

    public class RowDemo
    {
        public static void RowExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Ottenere il riferimento del primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un oggetto stile
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

            // Ottieni la prima riga
            Row row = worksheet.Cells.Rows[0];

            // Applica lo stile alla prima riga
            row.ApplyStyle(style, styleFlag);

            // Impostazione delle proprietà della riga
            row.Height = 20.0;
            row.IsHidden = false;
            row.IsCollapsed = false;
            row.GroupLevel = 1;
            row.IsHeightMatched = true;

            // Accesso alle celle nella riga
            Cell firstCell = row.FirstCell;
            Cell firstDataCell = row.FirstDataCell;
            Cell lastCell = row.LastCell;
            Cell lastDataCell = row.LastDataCell;

            // Verifica se la riga è vuota
            bool isBlank = row.IsBlank;

            // Verifica se la riga ha uno stile personalizzato
            bool hasCustomStyle = row.HasCustomStyle;

            // Ottenere l'indice della riga
            int rowIndex = row.Index;

            // Ottenere una cella per indice
            Cell cellByIndex = row.GetCellByIndex(0);

            // Ottenere lo stile della riga
            Style rowStyle = row.GetStyle();

            // Impostare lo stile della riga
            row.SetStyle(rowStyle);

            // Copiare le impostazioni da un'altra riga
            Row sourceRow = worksheet.Cells.Rows[1];
            row.CopySettings(sourceRow, true);

            // Enumerare le celle nella riga
            IEnumerator cellEnumerator = row.GetEnumerator();
            while (cellEnumerator.MoveNext())
            {
                Cell cell = (Cell)cellEnumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Salvataggio del file Excel
            workbook.Save("RowExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


