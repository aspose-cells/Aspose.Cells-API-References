---
title: "PivotField.GetPivotFilters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Ruft die Pivot-Filter des Pivot-Feldes ab"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/getpivotfilters/
---
## PivotField.GetPivotFilters method

Ruft die Pivot-Filter des Pivot-Feldes ab

```csharp
[Obsolete("Use PivotField.GetFilters() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetPivotFilters()
```

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.GetFilters(). Diese Methode wird 12 Monate später, seit November 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Collections;

    public class PivotFieldMethodGetPivotFiltersDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 8;
            worksheet.Cells["B5"].Value = 12;

            // Erstelle eine Pivot-Tabelle
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Pivot-Felder hinzufügen.
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Hole das Pivot-Feld
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Rufen Sie die GetPivotFilters-Methode auf (veraltet)
                ArrayList pivotFilters = pivotField.GetPivotFilters();
                
                Console.WriteLine($"Number of pivot filters: {pivotFilters.Count}");
                
                // Alternativ verwenden Sie die nicht veraltete GetFilters()-Methode
                PivotFilter[] filters = pivotField.GetFilters();
                Console.WriteLine($"Number of filters (non-obsolete method): {filters.Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPivotFilters method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("MethodGetPivotFiltersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


