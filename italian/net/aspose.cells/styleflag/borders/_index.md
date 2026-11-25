---
title: "StyleFlag.Borders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Tutte le impostazioni dei bordi verranno applicate"
type: docs
url: /it/net/aspose.cells/styleflag/borders/
---
## StyleFlag.Borders property

Tutte le impostazioni dei bordi verranno applicate.

```csharp
public bool Borders { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBordersDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea uno stile con impostazioni dei bordi
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].Color = System.Drawing.Color.Blue;

            // Crea un flag di stile e abilita i bordi
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // Applica lo stile alla cella A1 solo con i bordi
            cells["A1"].PutValue("Borders Demo");
            cells["A1"].SetStyle(style, styleFlag);

            // Salva la cartella di lavoro
            workbook.Save("BordersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


