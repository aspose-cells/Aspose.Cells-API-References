---
title: "Enum PivotGroupByType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Pivot.PivotGroupByType. Rappresenta il tipo di raggruppamento."
type: docs
url: /it/net/aspose.cells.pivot/pivotgroupbytype/
---
## PivotGroupByType enumeration

Rappresenta il tipo di raggruppamento.

```csharp
[Flags]
public enum PivotGroupByType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| RangeOfValues | `1` | Raggruppa per numeri. |
| Numbers | `1` | Raggruppa per numeri. |
| Seconds | `2` | Presenta il tipo di raggruppamento per secondi. |
| Minutes | `4` | Presenta il tipo di raggruppamento per minuti. |
| Hours | `8` | Presenta il tipo di raggruppamento per ore. |
| Days | `10` | Presenta il tipo di raggruppamento per giorni. |
| Months | `20` | Presenta il tipo di raggruppamento per mesi. |
| Quarters | `40` | Presenta il tipo di raggruppamento per trimestri. |
| Years | `80` | Presenta il tipo di raggruppamento per anni. |
| DateTimes | `FE` | Presenta tutti i tipi di raggruppamento di date e ore. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotGroupByTypeDemo
    {
        public static void PivotGroupByTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Date");
            Style style = workbook.CreateStyle();
            style.Number = 14;//m/d/yyy
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].SetStyle(style);

            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].SetStyle(style);

            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A4"].SetStyle(style);

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value field

            //TODO
            PivotField dateField = pivotTable.RowFields[0];

            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);

            // Accedi alle impostazioni del gruppo
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

            // Genera le impostazioni del gruppo
            Console.WriteLine("Group Type: " + groupSettings.Type);
            Console.WriteLine("Start Date: " + groupSettings.Start);
            Console.WriteLine("End Date: " + groupSettings.End);
            Console.WriteLine("Interval: " + groupSettings.Interval);
            Console.WriteLine("Is Grouped By Months: " + groupSettings.IsGroupedBy(PivotGroupByType.Months));

            // Salva la cartella di lavoro
            workbook.Save("PivotGroupByTypeExample.xlsx");
            
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


