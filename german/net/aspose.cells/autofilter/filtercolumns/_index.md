---
title: "AutoFilter.FilterColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Eigenschaft. Gibt die Sammlung der Filterspalten zurück"
type: docs
url: /de/net/aspose.cells/autofilter/filtercolumns/
---
## AutoFilter.FilterColumns property

Liest die Sammlung der Filterspalten.

```csharp
public FilterColumnCollection FilterColumns { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyFilterColumnsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Status");
            
            worksheet.Cells["A2"].PutValue("HR");
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["C2"].PutValue("Present");
            
            worksheet.Cells["A3"].PutValue("IT");
            worksheet.Cells["B3"].PutValue("Sarah");
            worksheet.Cells["C3"].PutValue("Absent");
            
            worksheet.Cells["A4"].PutValue("HR");
            worksheet.Cells["B4"].PutValue("Mike");
            worksheet.Cells["C4"].PutValue("Present");

            // Auto-Filter anwenden
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:C1";
            
            // Filterspalte 2 (Status) für "Present"-Werte
            autoFilter.Filter(2, "Present");
            
            // Zugriff auf die Filterspalte
            FilterColumn filterColumn = autoFilter.FilterColumns[2];
            
            // Speichere die Arbeitsmappe
            workbook.Save("AutoFilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [FilterColumnCollection](../../filtercolumncollection/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


