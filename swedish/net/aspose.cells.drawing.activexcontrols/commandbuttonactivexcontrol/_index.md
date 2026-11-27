---
title: "Klass CommandButtonActiveXControl"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.CommandButtonActiveXControl-klass. Representerar en kommandoknapp"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/
---
## CommandButtonActiveXControl class

Representerar en kommandoknapp.

```csharp
public class CommandButtonActiveXControl : ActiveXControl
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Accelerator](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/accelerator/) { get; set; } | Hämtar och anger acceleratortangenten för kontrollen. |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Hämtar och anger ole-färgen för bakgrunden.(ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Caption](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/caption/) { get; set; } | Hämtar och anger den beskrivande texten som visas på en kontroll. |
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
| [IsWordWrapped](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/iswordwrapped/) { get; set; } | Anger om innehållet i kontrollen automatiskt radbryts i slutet av en rad. |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Hämtar och anger den länkade cellen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Hämtar och anger listfyllningsområdet.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Hämtar och anger en anpassad ikon som ska visas som muspekaren för kontrollen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Hämtar och anger typen av ikon som visas som muspekaren för kontrollen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Picture](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/picture/) { get; set; } | Hämtar och anger bildens data. |
| [PicturePosition](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/pictureposition/) { get; set; } | Hämtar och anger placeringen av kontrollens bild i förhållande till dess rubrik. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Anger om en skugga ska visas.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TakeFocusOnClick](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/takefocusonclick/) { get; set; } | Anger om kontrollen får fokus när den klickas. |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Representerar hur texten som används av kontrollen ska justeras.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/type/) { get; } | Hämtar typen av ActiveX-kontrollen. |
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

    public class CommandButtonActiveXControlDemo
    {
        public static void CommandButtonActiveXControlExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en CommandButton ActiveX-kontroll i kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2,2,2, 100, 30);
            CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;

            // Ange egenskaper för CommandButton ActiveX-kontrollen
            commandButton.Caption = "Click Me";
            commandButton.PicturePosition = ControlPicturePositionType.Center;
            commandButton.Accelerator = 'C';
            commandButton.TakeFocusOnClick = true;
            commandButton.IsWordWrapped = true;
            commandButton.IsEnabled = true;
            commandButton.IsLocked = false;
            commandButton.IsTransparent = false;
            commandButton.IsAutoSize = false;
            commandButton.IMEMode = InputMethodEditorMode.NoControl;
            commandButton.TextAlign = TextAlignmentType.Center;
            commandButton.Width = 150;
            commandButton.Height = 50;
            commandButton.MousePointer = ControlMousePointerType.Default;
            commandButton.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
            commandButton.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
            commandButton.IsVisible = true;
            commandButton.Shadow = true;
            commandButton.LinkedCell = "A1";
            commandButton.ListFillRange = "A2:A10";

            // Spara arbetsboken
            workbook.Save("CommandButtonActiveXControlExample.xlsx");
            workbook.Save("CommandButtonActiveXControlExample.pdf");
        }
    }
}
```

### Se även

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


