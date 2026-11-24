---
title: "PivotField.FilterByDate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Filtert nach Datumswerten des Zeilen- oder Spalten-Pivotfelds."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/filterbydate/
---
## PivotField.FilterByDate method

Filtert nach Datumswerten des Zeilen‑ oder Spalten‑Pivot‑Felds.

```csharp
public PivotFilter FilterByDate(PivotFilterType type, DateTime dateTime1, DateTime dateTime2)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | PivotFilterType | Der Typ der zu filternden Daten. |
| dateTime1 | DateTime | Die Datumsbezeichnung der Filterbedingung |
| dateTime2 | DateTime | Die obere Begrenzungs-Datumsbezeichnung der Zwischenfilterbedingung |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByDateWithPivotFilterTypeDateTimeDateTimDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten mit Datumsangaben hinzufügen
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2020, 9, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2020, 10, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2021, 9, 16));
            worksheet.Cells["A5"].PutValue(new DateTime(2021, 11, 5));

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:A5", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Datumsfeld zum Spaltenbereich hinzufügen
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField pivotField = pivotTable.ColumnFields[fieldIndex];
            
            // Datumsfilter anwenden (September-Daten zwischen 2020-2021)
            pivotField.FilterByDate(PivotFilterType.September, new DateTime(2020, 1, 1), new DateTime(2021, 12, 31));
            
            // Pivot-Tabelle aktualisieren und berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Ergebnisse speichern
            workbook.Save("FilterByDateDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


