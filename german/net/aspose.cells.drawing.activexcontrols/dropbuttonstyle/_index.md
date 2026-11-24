---
title: "Enum DropButtonStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.DropButtonStyle enum. Stellt das Symbol dar, das auf der Drop-Schaltfläche angezeigt wird."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/dropbuttonstyle/
---
## DropButtonStyle enumeration

Stellt das auf der Dropdown-Schaltfläche angezeigte Symbol dar.

```csharp
public enum DropButtonStyle
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Plain | `0` | Zeigt eine Schaltfläche ohne Symbol an. |
| Arrow | `1` | Zeigt eine Schaltfläche mit einem nach unten zeigenden Pfeil an. |
| Ellipsis | `2` | Zeigt eine Schaltfläche mit einer Auslassung (...). |
| Reduce | `3` | Zeigt eine Schaltfläche mit einer horizontalen Linie, ähnlich einem Unterstrich, an. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class DropButtonStyleDemo
    {
        public static void DropButtonStyleExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein ComboBox ActiveX-Steuerelement zum Arbeitsblatt hinzu
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Setze Eigenschaften für die ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.ColumnCount = 1;
            comboBox.DropButtonStyle = DropButtonStyle.Arrow; // Set the drop button style to Arrow

            // Fügen Sie einige Elemente zur ComboBox hinzu
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            comboBox.ListFillRange = "A1:A4";

            // Speichere die Arbeitsmappe
            workbook.Save("DropButtonStyleExample.xlsx");
            workbook.Save("DropButtonStyleExample.pdf");

            // Geben Sie den verwendeten DropButtonStyle aus
            Console.WriteLine("DropButtonStyle set to: " + comboBox.DropButtonStyle);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


