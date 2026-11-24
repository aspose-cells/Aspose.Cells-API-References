---
title: "FindOptions.Style"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FindOptions‑Eigenschaft. Das Format, nach dem gesucht werden soll"
type: docs
url: /de/net/aspose.cells/findoptions/style/
---
## FindOptions.Style property

Das zu suchende Format.

```csharp
public Style Style { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Stil mit blauer Schrift
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Blue;

            // Wende den Stil auf die Zelle F2 an
            Cell cell = worksheet.Cells["F2"];
            cell.PutValue("SearchTarget");
            cell.SetStyle(style);

            // Erstelle Suchoptionen mit dem Stil
            FindOptions options = new FindOptions();
            options.Style = style;

            // Finde die Zelle mit passendem Stil
            Cell foundCell = worksheet.Cells.Find(null, null, options);

            // Gib den Namen der gefundenen Zelle aus
            Console.WriteLine("Cell found with matching style: " + foundCell?.Name);
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


