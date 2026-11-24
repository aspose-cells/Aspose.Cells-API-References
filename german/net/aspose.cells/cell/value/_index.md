---
title: "Cell.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt den in dieser Zelle enthaltenen Wert zurück bzw. setzt ihn"
type: docs
url: /de/net/aspose.cells/cell/value/
---
## Cell.Value property

Ermittelt/legt den in dieser Zelle enthaltenen Wert fest.

```csharp
public object Value { get; set; }
```

### Hinweise

Möglicher Typ:

null,

Boolean,

DateTime,

Double,

Integer

String.

Für int-Werte kann der Rückgabewert als Integer-Objekt oder als Double-Objekt erfolgen. Es gibt keine Garantie, dass der zurückgegebene Wert stets als derselbe Objekttyp beibehalten wird.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Werte über die Value-Eigenschaft festlegen
            cells[0, 0].Value = "Product ID";
            cells[0, 1].Value = "Product Name";
            
            // Nullwerte demonstrieren
            cells[0, 2].Value = null;
            cells[1, 0].Value = null;
            cells[1, 1].Value = null;
            cells[1, 2].Value = null;

            // Werte anzeigen
            Console.WriteLine("Cell[0,0] Value: " + cells[0, 0].Value);
            Console.WriteLine("Cell[0,1] Value: " + cells[0, 1].Value);
            Console.WriteLine("Cell[0,2] Value: " + (cells[0, 2].Value == null ? "null" : cells[0, 2].Value));
            Console.WriteLine("Cell[1,0] Value: " + (cells[1, 0].Value == null ? "null" : cells[1, 0].Value));
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


