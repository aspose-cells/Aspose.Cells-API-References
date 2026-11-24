---
title: "Cell.SharedStyleIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt den gemeinsam genutzten Stilindex der Zelle im Stilpool zurück."
type: docs
url: /de/net/aspose.cells/cell/sharedstyleindex/
---
## Cell.SharedStyleIndex property

Ermittelt den Index des geteilten Stils der Zelle im Stil‑Pool.

```csharp
public int SharedStyleIndex { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertySharedStyleIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie einen Stil und setzen Sie einige Eigenschaften.
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            // Den Stil auf Zelle A1 anwenden
            worksheet.Cells["A1"].SetStyle(style);

            // Abrufen des gemeinsamen Stilindex der Zelle A1.
            int sharedStyleIndex = worksheet.Cells["A1"].SharedStyleIndex;

            // Rufen Sie den Stil aus dem Stilpool anhand des Index ab.
            Style retrievedStyle = workbook.GetStyleInPool(sharedStyleIndex);

            // Geben Sie Stilinformationen aus, um zu überprüfen.
            Console.WriteLine("Font Name: " + retrievedStyle.Font.Name);
            Console.WriteLine("Font Size: " + retrievedStyle.Font.Size);
            Console.WriteLine("Is Bold: " + retrievedStyle.Font.IsBold);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


