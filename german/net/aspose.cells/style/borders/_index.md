---
title: "Style.Borders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt die BorderCollection des Stils zurück"
type: docs
url: /de/net/aspose.cells/style/borders/
---
## Style.Borders property

Gibt die [`BorderCollection`](../../bordercollection/) des Stils zurück.

```csharp
public BorderCollection Borders { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBordersDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hole Zelle und ihren Stil
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Setze verschiedene Rahmenstile
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Medium;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;
            
            // Wenden Sie den Stil auf die Zelle an
            cell.SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("BorderStylesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [BorderCollection](../../bordercollection/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


