---
title: "Klass ActiveXControlBase"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ActiveXControlBase klass. Representerar ActiveX-kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/
---
## ActiveXControlBase class

Representerar ActiveX-kontrollen.

```csharp
public abstract class ActiveXControlBase
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Hämtar och anger ole-färgen för bakgrunden. |
| virtual [Data](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/data/) { get; } | Hämtar och anger den binära datan för kontrollen. |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Hämtar och anger ole-färgen för förgrunden. |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Hämtar och anger kontrollens höjd i enheter av punkter. |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Anger om denna kontroll är synlig. |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Hämtar och anger den länkade cellen. |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Hämtar och anger listfyllningsområdet. |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Hämtar och anger en anpassad ikon som ska visas som muspekare för kontrollen. |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Hämtar och anger typen av ikon som visas som muspekare för kontrollen. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Anger om en skugga ska visas. |
| abstract [Type](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/type/) { get; } | Hämtar typen av ActiveX-kontrollen. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Hämtar och anger kontrollens bredd i enheter av punkter. |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Hämtar [`Workbook`](./workbook/) objektet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlBaseDemo
    {
        public static void ActiveXControlBaseExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ActiveX-kontroll på kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 100, 20);

            CheckBoxActiveXControl control = (CheckBoxActiveXControl)shape.ActiveXControl;
            control.Font.Size = 20;

            // Ange egenskaper för ActiveX-kontrollen
            control.Width = 150;
            control.Height = 30;
            control.MousePointer = ControlMousePointerType.Arrow;
            control.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Red);
            control.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Yellow);
            control.IsVisible = true;
            control.Shadow = true;
            control.LinkedCell = "A1";
            control.ListFillRange = "A2:A10";

            // Spara arbetsboken
            workbook.Save("ActiveXControlBaseExample.xlsx");
            workbook.Save("ActiveXControlBaseExample.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


