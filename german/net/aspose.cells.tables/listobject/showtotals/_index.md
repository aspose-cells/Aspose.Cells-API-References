---
title: "ListObject.ShowTotals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject‑Eigenschaft. Gibt an und legt fest, ob diese Tabelle die Summenzeile anzeigt"
type: docs
url: /de/net/aspose.cells.tables/listobject/showtotals/
---
## ListObject.ShowTotals property

Ermittelt und setzt, ob diese TAble die Summenzeile anzeigt.

```csharp
public bool ShowTotals { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTotalsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten hinzu, um eine Tabelle zu erstellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(8);

            // Ein Listenobjekt/Tabelle erstellen
            int index = worksheet.ListObjects.Add("A1", "B4", true);
            ListObject table = worksheet.ListObjects[index];

            // Aktiviere die Summenzeile und lege eine Berechnung fest
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Speichere die Arbeitsmappe
            workbook.Save("ListObjectShowTotalsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


