---
title: "Range.SetStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Wende den Zellstil an"
type: docs
url: /de/net/aspose.cells/range/setstyle/
---
## SetStyle(Style, bool) {#setstyle_1}

Wendet den Zellenstil an.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | Stil | Der Zellenstil. |
| explicitFlag | Boolean | True, überschreibt nur Formatierungen, die explizit gesetzt sind. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Style style = wb.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            
            Aspose.Cells.Range range = wb.Worksheets[0].Cells.CreateRange(0, 0, 1, 5);
            range.SetStyle(style, true);
            
            wb.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style) {#setstyle}

Legt den Stil des Bereichs fest.

```csharp
public void SetStyle(Style style)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | Stil | Das Style-Objekt. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie einen Stil
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.Font.Color = Color.Red;
            style.Font.Underline = FontUnderlineType.Single;

            // Wende den Stil auf eine Zelle an
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].SetStyle(style);

            // Erstelle einen Range und wende denselben Stil an
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "C3");
            range.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("RangeMethodSetStyleWithStyleDemo_output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


