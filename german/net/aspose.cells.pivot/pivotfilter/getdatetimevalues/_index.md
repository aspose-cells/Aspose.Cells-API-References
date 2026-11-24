---
title: "PivotFilter.GetDateTimeValues"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFilter-Methode. Gibt die Werte des Zahlenfilters zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotfilter/getdatetimevalues/
---
## PivotFilter.GetDateTimeValues method

Ermittelt die Werte des Zahlenfilters.

```csharp
public DateTime[] GetDateTimeValues()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetDateTimeValuesDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Date";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = DateTime.Now;
            cells["B2"].Value = 1000;
            cells["A3"].Value = DateTime.Now.AddDays(1);
            cells["B3"].Value = 2000;
            cells["A4"].Value = DateTime.Now.AddDays(2);
            cells["B4"].Value = 3000;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Fügen Sie ein Zeilenfeld hinzu und wenden Sie einen Datumsfilter an
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.BaseFields[0].FilterByDate(PivotFilterType.DateBetween, DateTime.Now, DateTime.Now.AddDays(1));
            
            // Rufen Sie den Filter ab und demonstrieren Sie GetDateTimeValues
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            DateTime[] dateValues = filter.GetDateTimeValues();
            
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("First Date Value: " + dateValues[0]);
            Console.WriteLine("Second Date Value: " + dateValues[1]);
        }
    }
}
```

### Siehe auch

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


