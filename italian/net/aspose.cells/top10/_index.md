---
title: "Classe Top10"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Top10. Descrivi la regola di formattazione condizionale Top10. Questa regola di formattazione condizionale evidenzia le celle i cui valori rientrano nella fascia dei primi N o degli ultimi N specificati"
type: docs
url: /it/net/aspose.cells/top10/
---
## Top10 class

Descrivi la regola di formattazione condizionale Top10. Questa regola di formattazione condizionale evidenzia le celle i cui valori rientrano nella fascia dei primi N o degli ultimi N, come specificato.

```csharp
public class Top10
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Top10](top10/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IsBottom](../../aspose.cells/top10/isbottom/) { get; set; } | Ottieni o imposta se una regola "top/bottom n" è una regola "bottom n". Il valore predefinito è false. |
| [IsPercent](../../aspose.cells/top10/ispercent/) { get; set; } | Ottieni o imposta se una regola "top/bottom n" è una regola "top/bottom n percent". Il valore predefinito è false. |
| [Rank](../../aspose.cells/top10/rank/) { get; set; } | Ottieni o imposta il valore di "n" in una regola di formattazione condizionale "top/bottom n". Se IsPercent è true, il valore deve essere compreso tra 0 e 100. Altrimenti deve essere compreso tra 0 e 1000. Il valore predefinito è 10. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class Top10Demo
    {
        public static void Top10Example()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiunge una formattazione condizionale vuota
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Imposta l'intervallo di formattazione condizionale
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Aggiunge condizione
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Impostazione delle proprietà
            Top10 top10 = fc.Top10;
            top10.IsPercent = false;
            top10.IsBottom = false;
            top10.Rank = 5;

            // Salvataggio del file Excel
            workbook.Save("Top10Example.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


