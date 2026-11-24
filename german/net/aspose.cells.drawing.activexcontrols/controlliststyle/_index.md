---
title: "Aufzählung ControlListStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlListStyle Aufzählung. Stellt das visuelle Erscheinungsbild der Liste in einer ListBox oder ComboBox dar"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/controlliststyle/
---
## ControlListStyle enumeration

Stellt das visuelle Erscheinungsbild der Liste in einer ListBox oder ComboBox dar.

```csharp
public enum ControlListStyle
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Plain | `0` | Zeigt eine Liste an, bei der der Hintergrund eines Elements hervorgehoben wird, wenn es ausgewählt ist. |
| Option | `1` | Zeigt eine Liste an, bei der neben jedem Eintrag ein Optionsfeld oder ein Kontrollkästchen den Auswahlstatus dieses Elements anzeigt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlListStyleDemo
    {
        public static void ControlListStyleExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["A4"].PutValue("Item 3");

            // Füge ein ComboBox ActiveX-Steuerelement zum Arbeitsblatt hinzu
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Setze Eigenschaften für die ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 3;
            comboBox.ColumnCount = 1;
            comboBox.ListStyle = ControlListStyle.Plain; // Set the ListStyle to Plain

            // Fügen Sie Elemente zur ComboBox hinzu
            comboBox.Value = "Item 1";
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = 1;

            // Fügen Sie ein ListBox ActiveX-Steuerelement zum Arbeitsblatt hinzu
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;

            // Legen Sie Eigenschaften für die ListBox fest
            listBox.ColumnCount = 1;
            listBox.ListStyle = ControlListStyle.Option; // Set the ListStyle to Option

            // Elemente zur ListBox hinzufügen
            listBox.Value = "Item 1";
            listBox.BoundColumn = 1;
            listBox.TextColumn = 1;

            // Speichere die Arbeitsmappe
            workbook.Save("ControlListStyleExample.xlsx");
            workbook.Save("ControlListStyleExample.pdf");

            // Ergebnisse ausgeben
            Console.WriteLine("ComboBox ListStyle: " + comboBox.ListStyle);
            Console.WriteLine("ListBox ListStyle: " + listBox.ListStyle);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


