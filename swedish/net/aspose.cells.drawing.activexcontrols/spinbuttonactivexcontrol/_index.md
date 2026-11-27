---
title: "Klass SpinButtonActiveXControl"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl-klass. Representerar SpinButton-kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/
---
## SpinButtonActiveXControl class

Representerar SpinButton-kontrollen.

```csharp
public class SpinButtonActiveXControl : ActiveXControl
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Hämtar och anger ole-färgen för bakgrunden.(ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Hämtar och anger den binära datan för kontrollen.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Representerar teckensnittet för kontrollen.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Hämtar och anger OLE-färgen för förgrunden.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Hämtar och anger höjden på kontrollen i enheter av punkter.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Hämtar och anger standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Indikerar om kontrollen automatiskt kommer att ändra storlek för att visa hela sitt innehåll.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Indikerar om kontrollen kan ta emot fokus och svara på användargenererade händelser.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Indikerar om data i kontrollen är låst för redigering.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Indikerar om kontrollen är transparent.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indikerar om den här kontrollen är synlig.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Hämtar och anger den länkade cellen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Hämtar och anger listfyllningsområdet.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Max](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max/) { get; set; } | Hämtar och anger det maximalt accepterade värdet. |
| [Min](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min/) { get; set; } | Hämtar och anger det minimalt accepterade värdet. |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Hämtar och anger en anpassad ikon som ska visas som muspekaren för kontrollen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Hämtar och anger typen av ikon som visas som muspekaren för kontrollen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Orientation](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation/) { get; set; } | Hämtar och anger om SpinButton eller ScrollBar är orienterad vertikalt eller horisontellt. |
| [Position](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position/) { get; set; } | Hämtar och anger värdet. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Anger om en skugga ska visas.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [SmallChange](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/smallchange/) { get; set; } | Hämtar och anger mängden som Position-egenskapen ändras med |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Representerar hur texten som används av kontrollen ska justeras.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type/) { get; } | Hämtar typen av ActiveX-kontrollen. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Hämtar och anger bredden på kontrollen i enheter av punkter.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Hämtar [`Workbook`](../activexcontrolbase/workbook/) objektet.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class SpinButtonActiveXControlDemo
    {
        public static void SpinButtonActiveXControlExample()
        {
            // Initiera en ny arbetsbok.
            Workbook workbook = new Workbook();

            // Lägg till en SpinButtonActiveXControl.
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.SpinButton, 1, 0, 1, 0, 100, 50);
            SpinButtonActiveXControl activeXControl = (SpinButtonActiveXControl)shape.ActiveXControl;

            // Ställa in egenskaper
            activeXControl.Min = 0;
            activeXControl.Max = 100;
            activeXControl.Position = 30;
            activeXControl.SmallChange = 5;

            if (activeXControl.Orientation == ControlScrollOrientation.Auto)
            {
                activeXControl.Orientation = ControlScrollOrientation.Horizontal;
            }

            activeXControl.IsEnabled = true;
            activeXControl.IsLocked = false;
            activeXControl.IsTransparent = false;
            activeXControl.IsAutoSize = true;
            activeXControl.IMEMode = InputMethodEditorMode.On;
            activeXControl.TextAlign = TextAlignmentType.Center;
            activeXControl.Width = 150;
            activeXControl.Height = 30;
            activeXControl.MousePointer = ControlMousePointerType.Default;
            activeXControl.ForeOleColor = 0x000000; // Black color
            activeXControl.BackOleColor = 0xFFFFFF; // White color
            activeXControl.IsVisible = true;
            activeXControl.Shadow = false;
            activeXControl.LinkedCell = "A1";
            activeXControl.ListFillRange = "A2:A10";

            // Spara arbetsboken
            workbook.Save("SpinButtonActiveXControlExample.xlsx");

            return;
        }
    }
}
```

### Se även

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


