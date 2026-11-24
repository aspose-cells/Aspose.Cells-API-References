---
title: "Style.SetPatternColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Methode. Legt die Hintergrundfarbe fest"
type: docs
url: /de/net/aspose.cells/style/setpatterncolor/
---
## Style.SetPatternColor method

Setzt die Hintergrundfarbe.

```csharp
public void SetPatternColor(BackgroundType pattern, Color color1, Color color2)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pattern | BackgroundType | Das Muster. |
| color1 | Farbe | Die Vordergrundfarbe. |
| color2 | Farbe | Die Hintergrundfarbe. Funktioniert nur, wenn das Muster nicht BackgroundType.None und BackgroundType.Solid ist. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetPatternColorWithBackgroundTypeColorColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.SetPatternColor(BackgroundType.Solid, Color.Red, Color.Blue);
            cell.SetStyle(style);
            
            workbook.Save("SetPatternColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


