---
title: "Classe PivotDateTimeRangeGroupSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotDateTimeRangeGroupSettings. Rappresenta il campo raggruppato per intervallo di data e ora"
type: docs
url: /it/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/
---
## PivotDateTimeRangeGroupSettings class

Rappresenta il campo raggruppato per intervallo di data e ora.

```csharp
public class PivotDateTimeRangeGroupSettings : PivotFieldGroupSettings
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [End](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/end/) { get; } | Ottiene la data e ora di fine del gruppo. |
| [GroupByTypes](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/groupbytypes/) { get; } | Ottiene i tipi di raggruppamento per data e ora. |
| [Interval](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/) { get; } | Ottiene l'interno del gruppo. |
| [Start](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/start/) { get; } | Ottiene la data e ora di inizio del gruppo. |
| override [Type](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/type/) { get; } | Ottiene il tipo di gruppo di data e ora. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [IsGroupedBy](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/isgroupedby/)(PivotGroupByType) | Verifica se il campo è raggruppato per tipo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotDateTimeRangeGroupSettingsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi dati di esempio con date
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
                worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
                worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["B4"].PutValue(30);

                // Crea tabella pivot
                int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Aggiungi campi alla tabella pivot
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Raggruppa il campo data per mesi
                PivotField dateField = pivotTable.RowFields[0];
                DateTime startDate = new DateTime(2023, 1, 1);
                DateTime endDate = new DateTime(2023, 12, 31);
                dateField.GroupBy(startDate, endDate, new PivotGroupByType[] { PivotGroupByType.Months }, 1, false);

                // Ottieni le impostazioni del gruppo
                PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

                // Visualizza le proprietà delle impostazioni del gruppo
                Console.WriteLine($"Group Type: {groupSettings.Type}");
                Console.WriteLine($"Start Date: {groupSettings.Start}");
                Console.WriteLine($"End Date: {groupSettings.End}");
                Console.WriteLine($"Interval: {groupSettings.Interval}");
                Console.WriteLine($"Group By Types: {string.Join(", ", groupSettings.GroupByTypes)}");

                // Verifica se è raggruppato per mesi
                bool isGroupedByMonths = groupSettings.IsGroupedBy(PivotGroupByType.Months);
                Console.WriteLine($"Is grouped by months: {isGroupedByMonths}");

                // Salva la cartella di lavoro
                workbook.Save("PivotDateTimeRangeGroupSettingsDemo.xlsx");
                Console.WriteLine("PivotDateTimeRangeGroupSettings demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in PivotDateTimeRangeGroupSettings demo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PivotFieldGroupSettings](../pivotfieldgroupsettings/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


