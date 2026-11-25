---
title: "Classe AboveAverage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.AboveAverage. Descrive la regola di formattazione condizionale AboveAverage. Questa regola di formattazione condizionale evidenzia le celle che sono sopra o sotto la media per tutti i valori nell'intervallo"
type: docs
url: /it/net/aspose.cells/aboveaverage/
---
## AboveAverage class

Descrivi la regola di formattazione condizionale AboveAverage. Questa regola di formattazione condizionale evidenzia le celle che sono al di sopra o al di sotto della media per tutti i valori nell'intervallo.

```csharp
public class AboveAverage
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [AboveAverage](aboveaverage/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IsAboveAverage](../../aspose.cells/aboveaverage/isaboveaverage/) { get; set; } | Ottieni o imposta il flag che indica se la regola è una regola "sopra la media". 'true' indica "sopra la media". Il valore predefinito è true. |
| [IsEqualAverage](../../aspose.cells/aboveaverage/isequalaverage/) { get; set; } | Ottieni o imposta il flag che indica se i criteri 'aboveAverage' e 'belowAverage' includono la media stessa o escludono quel valore. 'true' indica di includere il valore medio nei criteri. Il valore predefinito è false. |
| [StdDev](../../aspose.cells/aboveaverage/stddev/) { get; set; } | Ottieni o imposta il numero di deviazioni standard da includere sopra o sotto la media nella regola di formattazione condizionale. Il valore di input deve essere compreso tra 0 e 3 (inclusi 0 e 3). Impostare questo valore a 0 significa che stdDev non è impostato. Il valore predefinito è 0. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class AboveAverageDemo
    {
        public static void AboveAverageExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            // Aggiungi una raccolta di formattazione condizionale al foglio di lavoro
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            // Definisci l'area di celle a cui applicare la formattazione condizionale
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Aggiungi una condizione sopra la media alla raccolta
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            // Imposta il colore di sfondo per la condizione
            fc.Style.BackgroundColor = Color.Yellow;

            // Imposta le proprietà per la condizione sopra la media
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            Cells cells = worksheet.Cells;
            cells["A1"].Value = 20;
            cells["A2"].Value = 300;
            cells["A3"].Value = 40;
            cells["A4"].Value = 500;
            cells["A5"].Value = 6;
            cells["A6"].Value = 70;
            cells["A7"].Value = 8;
            cells["A8"].Value = 900;
            cells["A9"].Value = 10;

            cells["C1"].Value = 2;
            cells["C2"].Value = 3;
            cells["C3"].Value = 4;
            cells["C4"].Value = 5;
            cells["C5"].Value = 3;
            cells["C6"].Value = 2;
            cells["C7"].Value = 8;
            cells["C8"].Value = 300;
            cells["C9"].Value = 10;

            // Salva la cartella di lavoro
            workbook.Save("AboveAverageExample.xlsx");
            workbook.Save("AboveAverageExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


