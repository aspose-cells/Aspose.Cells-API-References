---
title: "AutoFilter.ShowFilterButton"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Eigenschaft. Gibt an, ob die AutoFilter-Schaltfläche für diese Spalte sichtbar ist"
type: docs
url: /de/net/aspose.cells/autofilter/showfilterbutton/
---
## AutoFilter.ShowFilterButton property

Gibt an, ob die AutoFilter-Schaltfläche für diese Spalte sichtbar ist.

```csharp
public bool ShowFilterButton { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyShowFilterButtonDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Ein Listenobjekt/Tabelle erstellen
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];

            // AutoFilter aktivieren und Filter-Schaltflächen anzeigen
            table.AutoFilter.ShowFilterButton = true;

            // Speichere die Arbeitsmappe
            workbook.Save("output_with_filter_buttons.xlsx");

            // Filter-Schaltflächen ausblenden
            table.AutoFilter.ShowFilterButton = false;
            workbook.Save("output_without_filter_buttons.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


