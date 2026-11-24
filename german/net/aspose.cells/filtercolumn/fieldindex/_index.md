---
title: "FilterColumn.FieldIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FilterColumn-Eigenschaft. Gibt den Spaltenversatz im Bereich zurück und setzt ihn"
type: docs
url: /de/net/aspose.cells/filtercolumn/fieldindex/
---
## FilterColumn.FieldIndex property

Liest und setzt den Spaltenversatz im Bereich.

```csharp
public int FieldIndex { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Employees");
            worksheet.Cells["A2"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["A3"].PutValue("Marketing");
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["A4"].PutValue("IT");
            worksheet.Cells["B4"].PutValue(12);

            // Auto-Filter anwenden
            worksheet.AutoFilter.Range = "A1:B4";
            
            // Filter zur ersten Spalte hinzufügen (Abteilung)
            worksheet.AutoFilter.AddFilter(0, "Sales");

            // Ermitteln Sie die Filterspalte
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            
            // FieldIndex-Eigenschaft demonstrieren
            Console.WriteLine("Filter is applied on column index: " + filterColumn.FieldIndex);
            
            // Aktualisieren und speichern
            worksheet.AutoFilter.Refresh();
            workbook.Save("FilterColumnFieldIndexDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


