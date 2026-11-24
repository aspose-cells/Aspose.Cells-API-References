---
title: "Style.HasBorders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Prüft, ob für den Stil Rahmen gesetzt wurden"
type: docs
url: /de/net/aspose.cells/style/hasborders/
---
## Style.HasBorders property

Überprüft, ob für den Stil Rahmen festgelegt wurden.

```csharp
public bool HasBorders { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHasBordersDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Greife auf Zelle A1 zu und prüfe, ob sie Rahmen hat (sollte standardmäßig false sein)
            Cell cellA1 = cells["A1"];
            Console.WriteLine("Cell A1 has borders: " + cellA1.GetStyle().HasBorders);

            // Erstelle einen Stil mit Rahmen
            Style styleWithBorders = workbook.CreateStyle();
            styleWithBorders.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            styleWithBorders.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Wende den Stil auf Zelle B1 an
            Cell cellB1 = cells["B1"];
            cellB1.SetStyle(styleWithBorders);

            // Prüfe, ob Zelle B1 Rahmen hat (sollte jetzt true sein)
            Console.WriteLine("Cell B1 has borders: " + cellB1.GetStyle().HasBorders);

            // Speichere die Arbeitsmappe
            workbook.Save("HasBordersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


