---
title: "Klasse UnknownControl"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.UnknownControl Klasse. Unbekannte Steuerung"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/unknowncontrol/
---
## UnknownControl class

Unbekanntes Steuerelement.

```csharp
public class UnknownControl : ActiveXControl
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Liest und schreibt die OLE-Farbe des Hintergrunds.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/unknowncontrol/data/) { get; } | Liest und setzt die Binärdaten des Steuerelements. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Stellt die Schriftart des Steuerelements dar.(Vererbt von [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Liest und schreibt die OLE-Farbe des Vordergrunds.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Liest und schreibt die Höhe des Steuerelements in Punkten.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Liest und schreibt den Standard‑Laufzeitmodus des Eingabemethoden-Editors für das Steuerelement, wenn es den Fokus erhält.(Vererbt von [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen.(Vererbt von [`ActiveXControl`](../activexcontrol/).) |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Gibt an, ob das Steuerelement den Fokus erhalten und auf benutzergenerierte Ereignisse reagieren kann.(Vererbt von [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind.(Vererbt von [`ActiveXControl`](../activexcontrol/).) |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Gibt an, ob das Steuerelement transparent ist.(Vererbt von [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Gibt an, ob dieses Steuerelement sichtbar ist.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Liest und schreibt die verknüpfte Zelle.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Liest und schreibt den Listenfüllbereich.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Liest und schreibt ein benutzerdefiniertes Symbol, das als Mauszeiger für das Steuerelement angezeigt wird.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Liest und schreibt den Typ des Symbols, das als Mauszeiger für das Steuerelement angezeigt wird.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Gibt an, ob ein Schatten angezeigt werden soll.(Vererbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird.(Geerbt von [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/unknowncontrol/type/) { get; } | Liest den Typ des ActiveX-Steuerelements. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Liest und setzt die Breite des Steuerelements in Punkt-Einheiten.(Geerbt von [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Liest das [`Workbook`](../activexcontrolbase/workbook/) Objekt.(Geerbt von [`ActiveXControlBase`](../activexcontrolbase/).) |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetRelationshipData](../../aspose.cells.drawing.activexcontrols/unknowncontrol/getrelationshipdata/)(string) | Ruft die zugehörigen Daten ab. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlsClassUnknownControlDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein unbekanntes ActiveX-Steuerelement zum Arbeitsblatt hinzu
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Unknown,
                0,  // topRow
                0,  // top
                0,  // leftColumn
                0,  // left
                100,// width
                50  // height
            );

            // Holen Sie die UnknownControl-Instanz aus der Form
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;
            unknownControl.IsVisible = true;

            // Speichere die Arbeitsmappe
            workbook.Save("UnknownControlDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


