---
title: "Klasse GroupFill"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.GroupFill Klasse. Gibt an, dass dieses Füllformat die Fülleigenschaften der Gruppe erben sollte"
type: docs
url: /de/net/aspose.cells.drawing/groupfill/
---
## GroupFill class

Stellt dar, dass dieses Füllformat die Fülleigenschaften der Gruppe erben sollte.

```csharp
public class GroupFill : Fill
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Geerbt von [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Liest den Hash‑Code. (Geerbt von [`Fill`](../fill/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGroupFillDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // GroupFill stellt keinen öffentlichen parameterlosen Konstruktor bereit.
                // Zu Demonstrationszwecken erhalten wir eine Referenz (null) des Typs.
                GroupFill groupFill = null;

                // Zeige, dass die Variable vom Typ GroupFill existiert.
                Console.WriteLine($"GroupFill variable declared. Type: {typeof(GroupFill).FullName}");

                // Speichere die Arbeitsmappe (obwohl wir sie nicht geändert haben, demonstriert dies einen vollständigen Arbeitsablauf)
                workbook.Save("GroupFillDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GroupFill: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


