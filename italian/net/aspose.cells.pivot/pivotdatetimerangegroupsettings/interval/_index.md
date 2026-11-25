---
title: "PivotDateTimeRangeGroupSettings.Interval"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotDateTimeRangeGroupSettings. Restituisce l'interno del gruppo"
type: docs
url: /it/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/
---
## PivotDateTimeRangeGroupSettings.Interval property

Ottiene l'interno del gruppo.

```csharp
public double Interval { get; }
```

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro con dati di esempio
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Aggiungi dati di data di esempio
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-5));
            dataSheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-4));
            dataSheet.Cells["A4"].PutValue(DateTime.Now.AddDays(-3));
            dataSheet.Cells["A5"].PutValue(DateTime.Now.AddDays(-2));
            dataSheet.Cells["A6"].PutValue(DateTime.Now.AddDays(-1));
            dataSheet.Cells["A7"].PutValue(DateTime.Now);

            // Aggiungi un foglio di lavoro pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            
            // Aggiungi tabella pivot
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:A7", 
                "A1", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Aggiungi il campo data all'area righe
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField dateField = pivotTable.RowFields[0];

            // Raggruppa per giorni con intervallo di 2
            dateField.GroupBy(1, false);
            PivotDateTimeRangeGroupSettings groupSettings = 
                (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            
            // Poiché Interval è di sola lettura, dobbiamo impostarlo durante il raggruppamento
            // L'intervallo è effettivamente impostato nei parametri del metodo GroupBy
            // Qui verifichiamo solo il valore dell'intervallo
            Console.WriteLine($"Grouping interval: {groupSettings.Interval} days");

            // Salva la cartella di lavoro
            workbook.Save("PivotDateTimeGroupingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


