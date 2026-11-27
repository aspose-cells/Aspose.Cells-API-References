---
title: "PivotDateTimeRangeGroupSettings.Interval"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotDateTimeRangeGroupSettings‑egenskap. Hämtar internvärdet för gruppen"
type: docs
url: /sv/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/
---
## PivotDateTimeRangeGroupSettings.Interval property

Hämtar interninformationen för gruppen.

```csharp
public double Interval { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDateTimeRangeGroupSettingsPropertyIntervalDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad med exempeldata
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Lägg till exempel på datumdata
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-5));
            dataSheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-4));
            dataSheet.Cells["A4"].PutValue(DateTime.Now.AddDays(-3));
            dataSheet.Cells["A5"].PutValue(DateTime.Now.AddDays(-2));
            dataSheet.Cells["A6"].PutValue(DateTime.Now.AddDays(-1));
            dataSheet.Cells["A7"].PutValue(DateTime.Now);

            // Lägg till ett pivottabellarbetsblad
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            
            // Lägg till pivottabell
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:A7", 
                "A1", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Lägg till datumfältet i radområdet
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField dateField = pivotTable.RowFields[0];

            // Gruppera efter dagar med ett intervall på 2
            dateField.GroupBy(1, false);
            PivotDateTimeRangeGroupSettings groupSettings = 
                (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            
            // Eftersom Interval är skrivskyddad, måste vi sätta den under gruppering
            // Intervallet sätts faktiskt i parametrarna för GroupBy‑metoden
            // Här verifierar vi bara intervalvärdet
            Console.WriteLine($"Grouping interval: {groupSettings.Interval} days");

            // Spara arbetsboken
            workbook.Save("PivotDateTimeGroupingDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


