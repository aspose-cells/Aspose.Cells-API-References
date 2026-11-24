---
title: "CustomFilter.Criteria"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomFilter-Eigenschaft. Gibt die Kriterien zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/customfilter/criteria/
---
## CustomFilter.Criteria property

Liest und setzt die Kriterien.

```csharp
public object Criteria { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomFilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Numbers");
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(5);
            worksheet.Cells["A5"].PutValue(9);
            worksheet.Cells["A6"].PutValue(3);

            // Auto-Filter anwenden
            worksheet.AutoFilter.Range = "A1:A6";
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // Benutzerdefinierten Filter hinzufügen
            int fieldIndex = 0;
            autoFilter.Custom(fieldIndex, FilterOperatorType.GreaterOrEqual, 5);
            
            // Abrufen der Filterspalte und Anzeige der Kriterien
            FilterColumn fc = autoFilter.FilterColumns[fieldIndex];
            CustomFilter cf = ((CustomFilterCollection)fc.Filter)[0];
            Console.WriteLine("Filter Criteria: " + cf.Criteria);
            
            // Filter aktualisieren
            autoFilter.Refresh();
            
            // Speichere die Arbeitsmappe
            workbook.Save("CustomFilterExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


