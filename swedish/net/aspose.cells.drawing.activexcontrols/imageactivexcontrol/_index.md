---
title: "Klass ImageActiveXControl"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl-klass. Representerar bildkontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/
---
## ImageActiveXControl class

Representerar bildkontrollen.

```csharp
public class ImageActiveXControl : ActiveXControl
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Hämtar och anger ole-färgen för bakgrunden.(ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [BorderOleColor](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderolecolor/) { get; set; } | Hämtar och anger ole-färgen för bakgrunden. |
| [BorderStyle](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderstyle/) { get; set; } | Hämtar och anger typen av ram som används av kontrollen. |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Hämtar och anger den binära datan för kontrollen.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Representerar teckensnittet för kontrollen.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Hämtar och anger OLE-färgen för förgrunden.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Hämtar och anger höjden på kontrollen i enheter av punkter.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Hämtar och anger standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| override [IsAutoSize](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/isautosize/) { get; set; } | Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Indikerar om kontrollen kan ta emot fokus och svara på användargenererade händelser.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Indikerar om data i kontrollen är låst för redigering.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| [IsTiled](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/istiled/) { get; set; } | Anger om bilden är upprepad över bakgrunden. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Indikerar om kontrollen är transparent.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indikerar om den här kontrollen är synlig.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Hämtar och anger den länkade cellen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Hämtar och anger listfyllningsområdet.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Hämtar och anger en anpassad ikon som ska visas som muspekaren för kontrollen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Hämtar och anger typen av ikon som visas som muspekaren för kontrollen.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Picture](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/picture/) { get; set; } | Hämtar och anger bildens data. |
| [PictureAlignment](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturealignment/) { get; set; } | Hämtar och anger bildens justering inom formuläret eller bilden. |
| [PictureSizeMode](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturesizemode/) { get; set; } | Hämtar och anger hur bilden ska visas. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Anger om en skugga ska visas.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [SpecialEffect](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/specialeffect/) { get; set; } | Hämtar och anger den speciella effekten för kontrollen. |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Representerar hur texten som används av kontrollen ska justeras.(Ärvd från [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/type/) { get; } | Hämtar typen av ActiveX-kontrollen. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Hämtar och anger bredden på kontrollen i enheter av punkter.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Hämtar [`Workbook`](../activexcontrolbase/workbook/) objektet.(Ärvd från [`ActiveXControlBase`](../activexcontrolbase/).) |

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
using System.IO;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlDemo
    {
        public static void RunDemo()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en Image ActiveX-kontroll i kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 0, 1, 1, 100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Ställ in egenskaper för Image ActiveX-kontrollen
            imageControl.IsAutoSize = true;
            imageControl.BorderOleColor = 0x000000; // Black border
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            imageControl.SpecialEffect = ControlSpecialEffectType.Flat;
            imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
            imageControl.IsTiled = false;

            // Läs in en bild från fil och tilldela den till kontrollen
            byte[] imageData = File.ReadAllBytes("ImageActiveXControlDemo.jpg");
            imageControl.Picture = imageData;

            // Spara arbetsboken
            workbook.Save("ImageActiveXControlDemo.xlsx");
            workbook.Save("ImageActiveXControlDemo.pdf");

            // Skriv ut resultaten
            Console.WriteLine("Image ActiveX Control added with the following properties:");
            Console.WriteLine($"IsAutoSize: {imageControl.IsAutoSize}");
            Console.WriteLine($"BorderOleColor: {imageControl.BorderOleColor}");
            Console.WriteLine($"BorderStyle: {imageControl.BorderStyle}");
            Console.WriteLine($"PictureSizeMode: {imageControl.PictureSizeMode}");
            Console.WriteLine($"SpecialEffect: {imageControl.SpecialEffect}");
            Console.WriteLine($"PictureAlignment: {imageControl.PictureAlignment}");
            Console.WriteLine($"IsTiled: {imageControl.IsTiled}");
        }
    }
}
```

### Se även

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


