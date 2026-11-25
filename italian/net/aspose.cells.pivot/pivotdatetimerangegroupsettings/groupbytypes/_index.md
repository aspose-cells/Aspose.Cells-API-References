---
title: "PivotDateTimeRangeGroupSettings.GroupByTypes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotDateTimeRangeGroupSettings. Restituisce i tipi di raggruppamento per data e ora"
type: docs
url: /it/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/groupbytypes/
---
## PivotDateTimeRangeGroupSettings.GroupByTypes property

Ottiene i tipi di raggruppamento per data e ora.

```csharp
public PivotGroupByType[] GroupByTypes { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotDateTimeRangeGroupSettingsPropertyGroupByTypesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con date
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            try
            {
                // Crea tabella pivot
                int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Aggiungi campi alla tabella pivot
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Raggruppa per data con più tipi di raggruppamento
                PivotField dateField = pivotTable.RowFields[0];
                DateTime startDate = new DateTime(2023, 1, 1);
                DateTime endDate = new DateTime(2023, 12, 31);
                PivotGroupByType[] groupTypes = new PivotGroupByType[]
                {
                    PivotGroupByType.Months,
                    PivotGroupByType.Quarters
                };
                dateField.GroupBy(startDate, endDate, groupTypes, 1, false);

                // Accedi alle impostazioni di gruppo e dimostra la proprietà GroupByTypes
                PivotDateTimeRangeGroupSettings groupSettings =
                    (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

                // Visualizza il valore della proprietà GroupByTypes
                Console.WriteLine("GroupByTypes values:");
                foreach (PivotGroupByType type in groupSettings.GroupByTypes)
                {
                    Console.WriteLine(type);
                }

                // Salva il risultato
                workbook.Save("GroupByTypesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


