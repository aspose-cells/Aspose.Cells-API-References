---
title: "Enum LookInType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.LookInType enum. Rappresenta il tipo di ricerca"
type: docs
url: /it/net/aspose.cells/lookintype/
---
## LookInType enumeration

Rappresenta il tipo di look-in.

```csharp
public enum LookInType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Formulas | `0` | Trova l'oggetto cercato dalla formula([`Formula`](../cell/formula/)) se la cella è una formula, altrimenti lo trova dal valore originale della cella (stesso di OriginalValues). |
| Values | `1` | Trova l'oggetto dal valore originale della cella([`Value`](../cell/value/)) e dal valore formattato([`StringValue`](../cell/stringvalue/)). |
| ValuesExcludeFormulaCell | `2` | Ignora le celle che sono formule. Per le celle che non sono formule, è lo stesso di Values. |
| Comments | `3` | Trova l'oggetto solo dal commento della cella. Ignora le celle che non hanno commenti. |
| OnlyFormulas | `4` | Ignora le celle che non sono formule. Per le celle che sono formule, trova l'oggetto cercato dalla formula([`Formula`](../cell/formula/)). |
| OriginalValues | `5` | Trova l'oggetto solo dal valore originale della cella. |
| FormattedValues | `6` | Trova l'oggetto solo dal valore formattato della cella([`StringValue`](../cell/stringvalue/)). |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassLookInTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati e formule
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].Formula = "=A1";
            worksheet.Cells["C1"].PutValue("Contains B1");

            // Trova la cella contenente la formula con "B1"
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            Cell foundCell = worksheet.Cells.Find("B1", null, options);

            // Restituisci il risultato
            if (foundCell != null)
            {
                Console.WriteLine($"Found cell at row: {foundCell.Row}, column: {foundCell.Column}");
                Console.WriteLine($"Cell value: {foundCell.StringValue}");
                Console.WriteLine($"Cell formula: {foundCell.Formula}");
            }
            else
            {
                Console.WriteLine("Cell not found");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


