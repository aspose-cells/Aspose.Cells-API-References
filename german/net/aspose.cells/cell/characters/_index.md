---
title: "Cell.Characters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt ein Characters-Objekt zurück, das einen Bereich von Zeichen im Zellentext darstellt"
type: docs
url: /de/net/aspose.cells/cell/characters/
---
## Cell.Characters method

Gibt ein Characters‑Objekt zurück, das einen Zeichenbereich innerhalb des Zellentextes darstellt.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | Int32 | Der Index des Beginns des Zeichens. |
| Länge | Int32 | Die Anzahl der Zeichen. |

### Rückgabewert

Characters-Objekt.

### Hinweise

Diese Methode funktioniert nur bei Zellen mit Zeichenkettenwert.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].PutValue("Helloworld");
            cells["A1"].Characters(5, 5).Font.IsBold = true;
            cells["A1"].Characters(5, 5).Font.Color = Color.Blue;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


