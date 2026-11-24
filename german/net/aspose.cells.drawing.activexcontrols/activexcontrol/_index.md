---
title: "Klasse ActiveXControl"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.ActiveXControl Klasse. Stellt das ActiveX-Steuerelement dar"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrol/
---
## ActiveXControl class

Stellt das ActiveX-Steuerelement dar.

```csharp
public abstract class ActiveXControl : ActiveXControlBase
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Liest und schreibt die OLE-Farbe des Hintergrunds.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Liest und setzt die Binärdaten des Steuerelements. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Stellt die Schriftart des Steuerelements dar. |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Liest und schreibt die OLE-Farbe des Vordergrunds.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Liest und schreibt die Höhe des Steuerelements in Punkten.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Liest und setzt den Standard‑Laufzeitmodus des Eingabemethoden-Editors für das Steuerelement, wenn es den Fokus erhält. |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Gibt an, ob das Steuerelement den Fokus erhalten und auf benutzergenerierte Ereignisse reagieren kann. |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Gibt an, ob das Steuerelement transparent ist. |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Gibt an, ob dieses Steuerelement sichtbar ist.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Liest und schreibt die verknüpfte Zelle.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Liest und schreibt den Listenfüllbereich.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Liest und schreibt ein benutzerdefiniertes Symbol, das als Mauszeiger für das Steuerelement angezeigt wird.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Liest und schreibt den Typ des Symbols, das als Mauszeiger für das Steuerelement angezeigt wird.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Gibt an, ob ein Schatten angezeigt werden soll.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird. |
| abstract [Type](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/type/) { get; } | Liest den Typ des ActiveX-Steuerelements.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Liest und setzt die Breite des Steuerelements in Punkt-Einheiten.(Geerbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Liest das [`Workbook`](../activexcontrolbase/workbook/) Objekt.(Geerbt von [`ActiveXControlBase`](../activexcontrolbase/).) |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassActiveXControlDemo
    {
        public static void Run()
        {
            // Arbeitsmappe erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // RadioButton ActiveX-Steuerelement hinzufügen
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.RadioButton, 
                1, 1,  // upper left row/column
                1, 1,  // upper left row/column offsets
                100, 30);  // width and height
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;

            // Eigenschaften festlegen
            radioButton.GroupName = "Sheet1";
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            radioButton.IsWordWrapped = true;
            radioButton.Caption = "OptionButton1";
            radioButton.PicturePosition = ControlPicturePositionType.AboveCenter;
            radioButton.SpecialEffect = ControlSpecialEffectType.Sunken;
            radioButton.IsEnabled = true;
            radioButton.IsTransparent = false;
            radioButton.IsAutoSize = false;
            radioButton.IMEMode = InputMethodEditorMode.NoControl;
            radioButton.Font.Name = "Calibri";
            radioButton.MousePointer = ControlMousePointerType.Default;

            // Speichere die Arbeitsmappe
            workbook.Save("ActiveXControlDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ActiveXControlBase](../activexcontrolbase/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


