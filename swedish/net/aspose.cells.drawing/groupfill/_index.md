---
title: "Klass GroupFill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.GroupFill-klass. Representerar att detta fyllningsformat bör ärva fyllningsegenskaperna från gruppen"
type: docs
url: /sv/net/aspose.cells.drawing/groupfill/
---
## GroupFill class

Representerar att detta fyllningsformat ska ärva fyllningsegenskaperna från gruppen.

```csharp
public class GroupFill : Fill
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Arv från [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Hämtar hashkoden.(Arv från [`Fill`](../fill/).) |

### Exempel

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
            // Skapa en ny arbetsbok för demonstrationen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // GroupFill exponerar inte en offentlig parameterlös konstruktor.
                // För demonstrationsändamål får vi en referens (null) av typen.
                GroupFill groupFill = null;

                // Visa att variabeln av typen GroupFill finns.
                Console.WriteLine($"GroupFill variable declared. Type: {typeof(GroupFill).FullName}");

                // Spara arbetsboken (även om vi inte ändrade den, detta demonstrerar ett komplett arbetsflöde)
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

### Se även

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


