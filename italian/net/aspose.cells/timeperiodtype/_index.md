---
title: "Enum TimePeriodType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.TimePeriodType. Utilizzato in una regola di formattazione condizionale FormatConditionType.TimePeriod. Questi sono periodi di tempo dinamici che cambiano in base alla data in cui la formattazione condizionale viene aggiornata / applicata"
type: docs
url: /it/net/aspose.cells/timeperiodtype/
---
## TimePeriodType enumeration

Utilizzato in una regola di formattazione condizionale FormatConditionType.TimePeriod. Questi sono periodi di tempo dinamici, che cambiano in base alla data in cui la formattazione condizionale viene aggiornata / applicata.

```csharp
public enum TimePeriodType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Today | `0` | Data odierna. |
| Yesterday | `1` | Data di ieri. |
| Tomorrow | `2` | Data di domani. |
| Last7Days | `3` | Una data negli ultimi sette giorni. |
| ThisMonth | `4` | Una data che si verifica in questo mese di calendario. |
| LastMonth | `5` | Una data che si verifica nell'ultimo mese del calendario. |
| NextMonth | `6` | Una data che si verifica nel prossimo mese del calendario. |
| ThisWeek | `7` | Una data che si verifica questa settimana. |
| LastWeek | `8` | Una data che si verifica la scorsa settimana. |
| NextWeek | `9` | Una data che si verifica la prossima settimana. |
| ThisYear | `10` | Una data che si verifica quest'anno. Solo per .ods. |
| LastYear | `11` | Una data che si verifica l'anno scorso. Solo per .ods. |
| NextYear | `12` | Una data che si verifica l'anno prossimo. Solo per .ods. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TimePeriodTypeDemo
    {
        public static void TimePeriodTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una regola di formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Definisci l'area della cella per la formattazione condizionale
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Aggiungi una condizione per il periodo di tempo
            int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;

            // Imposta il tipo di periodo di tempo
            fc.TimePeriod = TimePeriodType.Today;

            // Salva la cartella di lavoro
            workbook.Save("TimePeriodTypeExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


