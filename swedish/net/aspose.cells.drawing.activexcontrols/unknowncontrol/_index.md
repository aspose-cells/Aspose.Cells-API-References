---
title: "Klass UnknownControl"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.UnknownControl klass. Okänd kontroll"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/unknowncontrol/
---
## UnknownControl class

Okänd kontroll.

```csharp
public class UnknownControl : ActiveXControl
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Hämtar och anger ole-färgen för bakgrunden.(ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/unknowncontrol/data/) { get; } | Hämtar och anger den binära datan för kontrollen. |
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
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Hämtar och anger en anpassad ikon som ska visas som muspekaren för kontrollen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Hämtar och anger typen av ikon som visas som muspekaren för kontrollen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Anger om en skugga ska visas.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Representerar hur texten som används av kontrollen ska justeras.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/unknowncontrol/type/) { get; } | Hämtar typen av ActiveX-kontrollen. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Hämtar och anger bredden på kontrollen i enheter av punkter.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Hämtar [`Workbook`](../activexcontrolbase/workbook/) objektet.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetRelationshipData](../../aspose.cells.drawing.activexcontrols/unknowncontrol/getrelationshipdata/)(string) | Hämtar den relaterade datan. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en Okänd ActiveX-kontroll till kalkylbladet
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Unknown,
                0,  // topRow
                0,  // top
                0,  // leftColumn
                0,  // left
                100,// width
                50  // height
            );

            // Hämta UnknownControl-instansen från formen
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;
            unknownControl.IsVisible = true;

            // Spara arbetsboken
            workbook.Save("UnknownControlDemo.xlsx");
        }
    }
}
```

### Se även

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


