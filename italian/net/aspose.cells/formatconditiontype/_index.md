---
title: "Enum FormatConditionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.FormatConditionType. Tipo di regola di formattazione condizionale"
type: docs
url: /it/net/aspose.cells/formatconditiontype/
---
## FormatConditionType enumeration

Tipo di regola di formattazione condizionale.

```csharp
public enum FormatConditionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| CellValue | `1` | Questa regola di formattazione condizionale confronta il valore di una cella con il risultato calcolato di una formula, utilizzando un operatore. |
| Expression | `2` | Questa regola di formattazione condizionale contiene una formula da valutare. Quando il risultato della formula è vero, la cella viene evidenziata. |
| Top10 | `4` | Questa regola di formattazione condizionale evidenzia le celle i cui valori rientrano nella fascia superiore N o inferiore N, come specificato. |
| UniqueValues | `8` | Questa regola di formattazione condizionale evidenzia i valori unici nell'intervallo. |
| DuplicateValues | `16` | Questa regola di formattazione condizionale evidenzia i valori duplicati. |
| ContainsText | `32` | Questa regola di formattazione condizionale evidenzia le celle che contengono il testo specificato. Equivalente all'uso della funzione foglio SEARCH() per determinare se la cella contiene il testo. |
| NotContainsText | `64` | Questa regola di formattazione condizionale evidenzia le celle che non contengono il testo specificato. Equivalente all'uso della funzione foglio SEARCH() per determinare se la cella contiene o meno il testo. |
| BeginsWith | `128` | Questa regola di formattazione condizionale evidenzia le celle nell'intervallo che iniziano con il testo specificato. Equivalente all'uso della funzione foglio LEFT() e al confronto dei valori. |
| EndsWith | `256` | Questa regola di formattazione condizionale evidenzia le celle che terminano con il testo specificato. Equivalente all'uso della funzione foglio RIGHT() e al confronto dei valori. |
| ContainsBlanks | `512` | Questa regola di formattazione condizionale evidenzia le celle completamente vuote. Equivalente all'uso di LEN(TRIM()). Ciò significa che se la cella contiene solo caratteri che TRIM() rimuoverebbe, viene considerata vuota. Anche una cella vuota è considerata vuota. |
| NotContainsBlanks | `1024` | Questa regola di formattazione condizionale evidenzia le celle che non sono vuote. Equivalente all'uso di LEN(TRIM()). Ciò significa che se la cella contiene solo caratteri che TRIM() rimuoverebbe, viene considerata vuota. Anche una cella vuota è considerata vuota. |
| ContainsErrors | `2048` | Questa regola di formattazione condizionale evidenzia le celle con errori di formula. Equivalente all'uso della funzione foglio ISERROR() per determinare se c'è un errore di formula. |
| NotContainsErrors | `4096` | Questa regola di formattazione condizionale evidenzia le celle senza errori di formula. Equivalente all'uso della funzione foglio ISERROR() per determinare se c'è un errore di formula. |
| TimePeriod | `8192` | Questa regola di formattazione condizionale evidenzia le celle contenenti date nel periodo di tempo specificato. Il valore sottostante della cella viene valutato, quindi la cella non deve essere formattata come data per essere valutata. Ad esempio, con una cella contenente il valore 38913 la formattazione condizionale verrà applicata se la regola richiede un valore di 7/14/2006. |
| AboveAverage | `16384` | Questa regola di formattazione condizionale evidenzia le celle che sono sopra o sotto la media per tutti i valori nell'intervallo. |
| ColorScale | `32768` | Questa regola di formattazione condizionale crea una scala di colori graduale sulle celle. |
| DataBar | `65536` | Questa regola di formattazione condizionale visualizza una barra dati graduale nell'intervallo di celle. |
| IconSet | `131072` | Questa regola di formattazione condizionale applica icone alle celle in base ai loro valori. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionTypeDemo
    {
        public static void FormatConditionTypeExample()
        {
            // Crea un nuovo Workbook.
            Workbook workbook = new Workbook();

            // Ottieni il primo worksheet.
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiunge una formattazione condizionale vuota
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Imposta l'intervallo di formattazione condizionale.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Aggiunge una condizione per AboveAverage
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // Impostazione delle proprietà per AboveAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            // Aggiunge una condizione per CellValue
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = Color.Red;

            // Aggiunge una condizione per ContainsText
            int conditionIndex3 = fcs.AddCondition(FormatConditionType.ContainsText);
            FormatCondition fc3 = fcs[conditionIndex3];
            fc3.Text = "Sample";
            fc3.Style.BackgroundColor = Color.Green;

            // Salva il file Excel
            workbook.Save("FormatConditionTypeExample.xlsx");
            workbook.Save("FormatConditionTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


