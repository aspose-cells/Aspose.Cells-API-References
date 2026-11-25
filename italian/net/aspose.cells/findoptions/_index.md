---
title: "Class FindOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.FindOptions classe. Rappresenta le opzioni di ricerca"
type: docs
url: /it/net/aspose.cells/findoptions/
---
## FindOptions class

Rappresenta le opzioni di ricerca.

```csharp
public class FindOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [FindOptions](findoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CaseSensitive](../../aspose.cells/findoptions/casesensitive/) { get; set; } | Indica se la stringa cercata è sensibile al maiuscolo/minuscolo. |
| [ConvertNumericData](../../aspose.cells/findoptions/convertnumericdata/) { get; set; } | Ottiene o imposta un valore che indica se convertire il valore della stringa cercata in dati numerici. |
| [IsCaseSensitive](../../aspose.cells/findoptions/iscasesensitive/) { get; set; } | (**Obsolete.**) Indica se la stringa cercata è sensibile al maiuscolo/minuscolo. |
| [IsRangeSet](../../aspose.cells/findoptions/israngeset/) { get; } | Indica se l'intervallo cercato è impostato. |
| [LookAtType](../../aspose.cells/findoptions/lookattype/) { get; set; } | Guarda il tipo. |
| [LookInType](../../aspose.cells/findoptions/lookintype/) { get; set; } | Cerca nel tipo. |
| [RegexKey](../../aspose.cells/findoptions/regexkey/) { get; set; } | Indica se la chiave cercata è una regex. Se vero, la chiave cercata verrà considerata come regex e analizzata. Altrimenti la chiave verrà analizzata secondo le regole di MS Excel. |
| [SearchBackward](../../aspose.cells/findoptions/searchbackward/) { get; set; } | Indica se cercare all'indietro le celle. |
| [SearchNext](../../aspose.cells/findoptions/searchnext/) { get; set; } | (**Obsolete.**) Ordine di ricerca. Vero: cerca il successivo. Falso: cerca il precedente. |
| [SearchOrderByRows](../../aspose.cells/findoptions/searchorderbyrows/) { get; set; } | Indica se l'ordine di ricerca è per righe o colonne. |
| [Style](../../aspose.cells/findoptions/style/) { get; set; } | Il formato da cercare. |
| [ValueTypeSensitive](../../aspose.cells/findoptions/valuetypesensitive/) { get; set; } | Indica se il tipo di valore della cella cercata deve essere lo stesso della chiave cercata. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetRange](../../aspose.cells/findoptions/getrange/)() | Ottiene e imposta l'intervallo cercato. |
| [SetRange](../../aspose.cells/findoptions/setrange/)(CellArea) | Imposta l'intervallo cercato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsDemo
    {
        public static void FindOptionsExample()
        {
            // Istanzia l'oggetto cartella di lavoro
            Workbook workbook = new Workbook("FindOptionsExample_original.xlsx");

            // Ottieni la raccolta Cells
            Cells cells = workbook.Worksheets[0].Cells;

            // Istanzia l'oggetto FindOptions
            FindOptions findOptions = new FindOptions();

            // Crea un'area Cells
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.StartColumn = 0;
            ca.EndRow = 5;
            ca.EndColumn = 5;

            // Imposta l'area delle celle per le opzioni di ricerca
            findOptions.SetRange(ca);

            // Imposta le proprietà di ricerca
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // Trova la cella con valore 0
            Cell cell = cells.Find(0, null, findOptions);

            if (cell != null)
            {
                Console.WriteLine("Cell found at: " + cell.Name);
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


