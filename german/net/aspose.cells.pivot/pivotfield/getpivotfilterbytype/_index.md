---
title: "PivotField.GetPivotFilterByType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Gibt den Pivot-Filter des Pivot-Feldes nach Typ zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/getpivotfilterbytype/
---
## PivotField.GetPivotFilterByType method

Liest den Pivot‑Filter des Pivot‑Feldes nach Typ

```csharp
public PivotFilter GetPivotFilterByType(PivotFilterType type)
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetPivotFilterByTypeWithPivotFilterTypeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["A5"].Value = "Apple";
            
            sheet.Cells["B1"].Value = "Count";
            sheet.Cells["B2"].Value = 1;
            sheet.Cells["B3"].Value = 2;
            sheet.Cells["B4"].Value = 3;
            sheet.Cells["B5"].Value = 4;

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Zeilenfeld und Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Zählfilter anwenden
            PivotField rowField = pivotTable.RowFields[0];
            rowField.FilterTop10(0, PivotFilterType.Count, true, 2);
            
            // Den Zählfilter abrufen
            PivotFilter filter = rowField.GetPivotFilterByType(PivotFilterType.Count);
            
            // Filterdetails ausgeben
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Value Field Index: " + filter.ValueFieldIndex);
            Console.WriteLine("Auto Filter: " + filter.AutoFilter);
            
            wb.Save("PivotFilterExample.xlsx");
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


