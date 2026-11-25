---
title: "Enum OperatorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.OperatorType. Rappresenta il tipo di operatore del formato condizionale e della convalida dei dati"
type: docs
url: /it/net/aspose.cells/operatortype/
---
## OperatorType enumeration

Rappresenta il tipo di operatore della formattazione condizionale e della convalida dei dati.

```csharp
public enum OperatorType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Between | `0` | Rappresenta l'operatore Between del formato condizionale e della convalida dei dati. |
| Equal | `1` | Rappresenta l'operatore Equal del formato condizionale e della convalida dei dati. |
| GreaterThan | `2` | Rappresenta l'operatore GreaterThan del formato condizionale e della convalida dei dati. |
| GreaterOrEqual | `3` | Rappresenta l'operatore GreaterOrEqual del formato condizionale e della convalida dei dati. |
| LessThan | `4` | Rappresenta l'operatore LessThan del formato condizionale e della convalida dei dati. |
| LessOrEqual | `5` | Rappresenta l'operatore LessOrEqual del formato condizionale e della convalida dei dati. |
| None | `6` | Rappresenta nessun confronto. |
| NotBetween | `7` | Rappresenta l'operatore NotBetween del formato condizionale e della convalida dei dati. |
| NotEqual | `8` | Rappresenta l'operatore NotEqual del formato condizionale e della convalida dei dati. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OperatorTypeDemo
    {
        public static void OperatorTypeExample()
        {
            // Crea una nuova Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una formattazione condizionale vuota
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Imposta l'intervallo di formattazione condizionale
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Aggiungi una condizione con OperatorType.Between
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "100");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Aggiungi un'altra condizione con OperatorType.GreaterThan
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", null);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = System.Drawing.Color.Green;

            // Salva la cartella di lavoro
            workbook.Save("OperatorTypeExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


