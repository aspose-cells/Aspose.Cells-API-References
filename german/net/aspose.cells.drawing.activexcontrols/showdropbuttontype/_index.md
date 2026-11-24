---
title: "Enum ShowDropButtonType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.ShowDropButtonType enum. Gibt an, wann die Drop-Schaltfläche angezeigt werden soll."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/showdropbuttontype/
---
## ShowDropButtonType enumeration

Gibt an, wann die Dropdown-Schaltfläche angezeigt wird

```csharp
public enum ShowDropButtonType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Never | `0` | Die Drop-Schaltfläche niemals anzeigen. |
| Focus | `1` | Die Drop-Schaltfläche anzeigen, wenn das Steuerelement den Fokus hat. |
| Always | `2` | Die Drop-Schaltfläche immer anzeigen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ShowDropButtonTypeDemo
    {
        public static void ShowDropButtonTypeExample()
        {
            // Initialisieren Sie ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein ComboBox ActiveX-Steuerelement zum Arbeitsblatt hinzu
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Eigenschaften für das ComboBox‑ActiveX‑Steuerelement festlegen
            comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus; // Show drop button when the control has focus
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.IsEditable = true;

            // Fügen Sie einige Elemente zur ComboBox hinzu
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Speichere die Arbeitsmappe
            workbook.Save("ShowDropButtonTypeExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


