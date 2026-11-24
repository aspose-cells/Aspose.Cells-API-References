---
title: "StyleFlag.Locked"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Locked-Einstellung wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/locked/
---
## StyleFlag.Locked property

Die gesperrte Einstellung wird angewendet.

```csharp
public bool Locked { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLockedDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Erstellen Sie einen Stil und setzen Sie dessen Locked-Eigenschaft
            Style style = workbook.CreateStyle();
            style.IsLocked = true;

            // Erstellen Sie ein Style-Flag und aktivieren Sie das Locked-Flag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Locked = true;

            // Den Stil auf Zelle A1 anwenden
            Cell cell = cells["A1"];
            cell.SetStyle(style, styleFlag);

            // Überprüfen Sie den gesperrten Status
            Console.WriteLine("Cell A1 is locked: " + cell.GetStyle().IsLocked);

            // Schützen Sie das Arbeitsblatt, um die Sperrwirkung zu sehen
            worksheet.Protect(ProtectionType.All);

            // Versuchen Sie, die gesperrte Zelle zu ändern (wirft eine Ausnahme, wenn das Arbeitsblatt geschützt ist)
            try
            {
                cell.PutValue("Test");
                Console.WriteLine("Cell modified successfully (worksheet not properly protected)");
            }
            catch
            {
                Console.WriteLine("Could not modify locked cell (worksheet protected)");
            }
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


