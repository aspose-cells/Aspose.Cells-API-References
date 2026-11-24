---
title: "Enum ControlBorderType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlBorderType enum. Stellt den Randtyp des ActiveX‑Steuerelements dar"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/controlbordertype/
---
## ControlBorderType enumeration

Stellt den Rahmentyp des ActiveX-Steuerelements dar.

```csharp
public enum ControlBorderType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Kein Rahmen. |
| Single | `1` | Die einzelne Zeile. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;

    public class ControlBorderTypeDemo
    {
        public static void ControlBorderTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein ComboBox ActiveX-Steuerelement zum Arbeitsblatt hinzu
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Eigenschaften für das ComboBox‑ActiveX‑Steuerelement festlegen
            comboBox.MaxLength = 100;
            comboBox.ListWidth = 150;
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = 1;
            comboBox.ColumnCount = 1;
            comboBox.ListRows = 5;
            comboBox.MatchEntry = ControlMatchEntryType.Complete;
            comboBox.DropButtonStyle = DropButtonStyle.Arrow;
            comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Always;
            comboBox.ListStyle = ControlListStyle.Plain;
            comboBox.BorderStyle = ControlBorderType.Single; // Set border style to Single
            comboBox.BorderOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Black);
            comboBox.SpecialEffect = ControlSpecialEffectType.Flat;
            comboBox.IsEditable = true;
            comboBox.ShowColumnHeads = false;
            comboBox.IsDragBehaviorEnabled = false;
            comboBox.EnterFieldBehavior = true;
            comboBox.IsAutoWordSelected = false;
            comboBox.SelectionMargin = false;
            comboBox.Value = "Sample Text";
            comboBox.HideSelection = true;
            comboBox.ColumnWidths = 100;

            // Speichere die Arbeitsmappe
            workbook.Save("ControlBorderTypeExample.xlsx");
            workbook.Save("ControlBorderTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


