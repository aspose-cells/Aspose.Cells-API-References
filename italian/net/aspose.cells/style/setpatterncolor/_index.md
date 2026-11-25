---
title: "Style.SetPatternColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Style. Imposta il colore di sfondo"
type: docs
url: /it/net/aspose.cells/style/setpatterncolor/
---
## Style.SetPatternColor method

Imposta il colore di sfondo.

```csharp
public void SetPatternColor(BackgroundType pattern, Color color1, Color color2)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| modello | BackgroundType | Il modello. |
| color1 | Color | Il colore di primo piano. |
| color2 | Color | Il colore di sfondo. Funziona solo quando il pattern non è BackgroundType.None e BackgroundType.Solid. |

### Esempi

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

### Vedi anche

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


