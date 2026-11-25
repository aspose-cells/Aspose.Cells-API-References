---
title: "PivotDateTimeRangeGroupSettings.Start"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotDateTimeRangeGroupSettings. Restituisce la data e ora di inizio del gruppo"
type: docs
url: /it/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/start/
---
## PivotDateTimeRangeGroupSettings.Start property

Ottiene la data e ora di inizio del gruppo.

```csharp
public DateTime Start { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDateTimeRangeGroupSettingsPropertyStartDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
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

            // Aggiungi campi
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Raggruppa per intervallo di date
            PivotField dateField = pivotTable.RowFields[0];
            DateTime startDate = new DateTime(2023, 1, 1);
            DateTime endDate = new DateTime(2023, 12, 31);
            dateField.GroupBy(startDate, endDate, new PivotGroupByType[] { PivotGroupByType.Months }, 1, false);

            // Accedi alle impostazioni di gruppo e dimostra la proprietà Start
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            Console.WriteLine("Group Start Date: " + groupSettings.Start);

            // Salva cartella di lavoro
            workbook.Save("PivotDateTimeRangeGroupSettingsStartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


