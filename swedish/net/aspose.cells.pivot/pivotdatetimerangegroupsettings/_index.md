---
title: "Klass PivotDateTimeRangeGroupSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotDateTimeRangeGroupSettings-klass. Representerar fältet grupperat efter datum- och tidsintervall"
type: docs
url: /sv/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/
---
## PivotDateTimeRangeGroupSettings class

Representerar fältet grupperat efter datum- och tidsintervall.

```csharp
public class PivotDateTimeRangeGroupSettings : PivotFieldGroupSettings
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [End](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/end/) { get; } | Hämtar slutdatum och tid för gruppen. |
| [GroupByTypes](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/groupbytypes/) { get; } | Hämtar typerna av gruppering efter datum och tid. |
| [Interval](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/) { get; } | Hämtar interninformationen för gruppen. |
| [Start](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/start/) { get; } | Hämtar startdatum och tid för gruppen. |
| override [Type](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/type/) { get; } | Hämtar datatidsgruppens typ. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [IsGroupedBy](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/isgroupedby/)(PivotGroupByType) | Kontrollera om fältet är grupperat efter typen. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till exempeldata med datum
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
                worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
                worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["B4"].PutValue(30);

                // Skapa pivottabell
                int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Lägg till fält i pivottabell
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Gruppera datumfältet efter månader
                PivotField dateField = pivotTable.RowFields[0];
                DateTime startDate = new DateTime(2023, 1, 1);
                DateTime endDate = new DateTime(2023, 12, 31);
                dateField.GroupBy(startDate, endDate, new PivotGroupByType[] { PivotGroupByType.Months }, 1, false);

                // Hämta gruppinställningarna
                PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

                // Visa egenskaper för gruppinställningar
                Console.WriteLine($"Group Type: {groupSettings.Type}");
                Console.WriteLine($"Start Date: {groupSettings.Start}");
                Console.WriteLine($"End Date: {groupSettings.End}");
                Console.WriteLine($"Interval: {groupSettings.Interval}");
                Console.WriteLine($"Group By Types: {string.Join(", ", groupSettings.GroupByTypes)}");

                // Kontrollera om grupperad efter månader
                bool isGroupedByMonths = groupSettings.IsGroupedBy(PivotGroupByType.Months);
                Console.WriteLine($"Is grouped by months: {isGroupedByMonths}");

                // Spara arbetsboken
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

### Se även

* class [PivotFieldGroupSettings](../pivotfieldgroupsettings/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


