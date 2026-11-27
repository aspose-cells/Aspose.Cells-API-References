---
title: "Klass ActiveXControl"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ActiveXControl-klass. Representerar ActiveX-kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrol/
---
## ActiveXControl class

Representerar ActiveX-kontrollen.

```csharp
public abstract class ActiveXControl : ActiveXControlBase
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Hämtar och anger ole-färgen för bakgrunden.(ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Hämtar och anger den binära datan för kontrollen. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Representerar teckensnittet för kontrollen. |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Hämtar och anger OLE-färgen för förgrunden.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Hämtar och anger höjden på kontrollen i enheter av punkter.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Hämtar och anger standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus. |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser. |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Anger om data i kontrollen är låst för redigering. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Anger om kontrollen är transparent. |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indikerar om den här kontrollen är synlig.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Hämtar och anger den länkade cellen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Hämtar och anger listfyllningsområdet.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Hämtar och anger en anpassad ikon som ska visas som muspekaren för kontrollen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Hämtar och anger typen av ikon som visas som muspekaren för kontrollen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Anger om en skugga ska visas.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Representerar hur texten som används av kontrollen ska justeras. |
| abstract [Type](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/type/) { get; } | Hämtar typen av ActiveX-kontrollen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Hämtar och anger bredden på kontrollen i enheter av punkter.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Hämtar [`Workbook`](../activexcontrolbase/workbook/) objektet.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |

### Exempel

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
            // Skapa arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till RadioButton ActiveX-kontroll
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.RadioButton, 
                1, 1,  // upper left row/column
                1, 1,  // upper left row/column offsets
                100, 30);  // width and height
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;

            // Ställ in egenskaper
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

            // Spara arbetsboken
            workbook.Save("ActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* class [ActiveXControlBase](../activexcontrolbase/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


