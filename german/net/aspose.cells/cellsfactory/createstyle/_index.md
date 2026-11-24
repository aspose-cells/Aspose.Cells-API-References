---
title: "CellsFactory.CreateStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsFactory-Methode. Erstellt einen neuen Stil"
type: docs
url: /de/net/aspose.cells/cellsfactory/createstyle/
---
## CellsFactory.CreateStyle method

Erstellt einen neuen Stil.

```csharp
public Style CreateStyle()
```

### Rückgabewert

Gibt ein Stilobjekt zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsFactoryMethodCreateStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstelle einen Stil mit CellsFactory
            Style style = new CellsFactory().CreateStyle();
            
            // Rand-Eigenschaften für den Stil festlegen
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thick, Color.Black);
            
            // Wende den Stil auf eine Zelle an
            workbook.Worksheets[0].Cells["A1"].Value = "Hello World";
            workbook.Worksheets[0].Cells["A1"].SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [CellsFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


