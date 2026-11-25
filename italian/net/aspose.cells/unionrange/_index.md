---
title: "Classe UnionRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.UnionRange. Rappresenta un intervallo unito"
type: docs
url: /it/net/aspose.cells/unionrange/
---
## UnionRange class

Rappresenta un intervallo di unione.

```csharp
public class UnionRange : IEnumerable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CellCount](../../aspose.cells/unionrange/cellcount/) { get; } | Ottiene il conteggio totale delle celle nell'intervallo. |
| [ColumnCount](../../aspose.cells/unionrange/columncount/) { get; } | Ottiene il conteggio delle righe nell'intervallo. |
| [FirstColumn](../../aspose.cells/unionrange/firstcolumn/) { get; } | Ottiene l'indice della prima colonna dell'intervallo. |
| [FirstRow](../../aspose.cells/unionrange/firstrow/) { get; } | Ottiene l'indice della prima riga dell'intervallo. |
| [HasRange](../../aspose.cells/unionrange/hasrange/) { get; } | Indica se questo ha un intervallo. |
| [Hyperlinks](../../aspose.cells/unionrange/hyperlinks/) { get; } | Ottiene tutti i collegamenti ipertestuali nell'intervallo. |
| [Name](../../aspose.cells/unionrange/name/) { get; set; } | Ottiene o imposta il nome dell'intervallo. |
| [RangeCount](../../aspose.cells/unionrange/rangecount/) { get; } | Ottiene il conteggio degli intervalli. |
| [Ranges](../../aspose.cells/unionrange/ranges/) { get; } | Ottiene tutti gli intervalli di unione. |
| [RefersTo](../../aspose.cells/unionrange/refersto/) { get; } | Ottiene a cosa si riferisce l'intervallo. |
| [RowCount](../../aspose.cells/unionrange/rowcount/) { get; } | Ottiene il conteggio delle righe nell'intervallo. |
| [Value](../../aspose.cells/unionrange/value/) { get; set; } | Ottiene e imposta i valori dell'intervallo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ApplyStyle](../../aspose.cells/unionrange/applystyle/)(Style, StyleFlag) | Applica formati a un intero intervallo. |
| [Copy](../../aspose.cells/unionrange/copy/)(UnionRange, PasteOptions) | Copia l'intervallo con le opzioni incolla speciale. |
| [GetEnumerator](../../aspose.cells/unionrange/getenumerator/)() | Ottiene l'enumeratore per le celle in questo Intervallo. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect)(Range[]) | Interseca un altro intervallo. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_2)(string) | Interseca un altro intervallo. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_1)(UnionRange) | Interseca un altro intervallo. |
| [Merge](../../aspose.cells/unionrange/merge/)() | Combina un intervallo di celle in una singola cella. |
| [PutValue](../../aspose.cells/unionrange/putvalue/)(string, bool, bool) | Inserisce un valore nell'intervallo; se opportuno il valore sarà convertito in un altro tipo di dati e il formato numerico della cella verrà ripristinato. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders)(CellBorderType, Color) | Imposta i bordi esterni attorno a un intervallo di celle con lo stesso stile e colore di bordo. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders_1)(CellBorderType[], Color[]) | Imposta i bordi esterni attorno a un intervallo di celle. |
| [SetStyle](../../aspose.cells/unionrange/setstyle/)(Style) | Imposta lo stile dell'intervallo. |
| [Union](../../aspose.cells/unionrange/union/#union)(Range[]) | Unisci gli intervalli. |
| [Union](../../aspose.cells/unionrange/union/#union_2)(string) | Unisci un altro intervallo. |
| [Union](../../aspose.cells/unionrange/union/#union_1)(UnionRange) | Unisci un altro intervallo. |
| [UnMerge](../../aspose.cells/unionrange/unmerge/)() | Separa le celle unite di questo intervallo. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassUnionRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo di unione usando l'API corretta
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A10,C1:C10", 0);
            
            // Imposta il valore per l'intero intervallo di unione
            unionRange.Value = "Test";
            
            // Applica lo stile all'intervallo di unione
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // Salva la cartella di lavoro
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


