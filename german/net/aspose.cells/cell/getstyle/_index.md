---
title: "Cell.GetStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt den Zellenstil zurück"
type: docs
url: /de/net/aspose.cells/cell/getstyle/
---
## GetStyle() {#getstyle}

Liefert den Zellenstil.

```csharp
public Style GetStyle()
```

### Rückgabewert

Stil-Objekt.

### Hinweise

Um den Stil der Zelle zu ändern, rufen Sie bitte die Methode Cell.SetStyle() auf, nachdem Sie das zurückgegebene Stil-Objekt geändert haben. Diese Methode ist identisch mit `GetStyle` mit dem Wert true für den Parameter.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Verschiedene vertikale Ausrichtungen für Zellen festlegen
            cells["A1"].PutValue("Bottom Alignment");
            cells["A1"].GetStyle().VerticalAlignment = TextAlignmentType.Bottom;

            cells["A2"].PutValue("Center Alignment");
            cells["A2"].GetStyle().VerticalAlignment = TextAlignmentType.Center;

            cells["A3"].PutValue("Distributed Alignment");
            cells["A3"].GetStyle().VerticalAlignment = TextAlignmentType.Distributed;

            cells["A4"].PutValue("Justify Alignment");
            cells["A4"].GetStyle().VerticalAlignment = TextAlignmentType.Justify;

            cells["A5"].PutValue("Top Alignment");
            cells["A5"].GetStyle().VerticalAlignment = TextAlignmentType.Top;

            // Demonstriere die GetStyle()-Methode
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("A2 Vertical Alignment: " + cells["A2"].GetStyle().VerticalAlignment);
            Console.WriteLine("A3 Vertical Alignment: " + cells["A3"].GetStyle().VerticalAlignment);
            Console.WriteLine("A4 Vertical Alignment: " + cells["A4"].GetStyle().VerticalAlignment);
            Console.WriteLine("A5 Vertical Alignment: " + cells["A5"].GetStyle().VerticalAlignment);
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetStyle(bool) {#getstyle_1}

Wenn checkBorders true ist, prüfe, ob die Rahmen anderer Zellen den Stil dieser Zelle beeinflussen.

```csharp
public Style GetStyle(bool checkBorders)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| checkBorders | Boolean | Überprüfe die Ränder anderer Zellen |

### Rückgabewert

Stil-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greife auf eine Zelle zu und setze einige Beispieldaten
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(123.456);

            // Hole den Zellenstil, ohne von Zeile/Spalte zu erben (Parameter false)
            Style style = cell.GetStyle(false);
            
            // Stil ändern
            style.Custom = "0.000";
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.None;

            // Wende den geänderten Stil auf die Zelle an
            cell.SetStyle(style);

            // Überprüfe die Stiländerungen
            Console.WriteLine("Number Format: " + cell.GetStyle(false).Custom);
            Console.WriteLine("Top Border Style: " + cell.GetStyle(false).Borders[BorderType.TopBorder].LineStyle);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


