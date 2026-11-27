---
title: "Enum ShowDropButtonType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ShowDropButtonType enum. Anger när du ska visa nedrullningsknappen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/showdropbuttontype/
---
## ShowDropButtonType enumeration

Anger när drop button ska visas

```csharp
public enum ShowDropButtonType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Never | `0` | Visa aldrig nedrullningsknappen. |
| Focus | `1` | Visa nedrullningsknappen när kontrollen har fokus. |
| Always | `2` | Visa alltid nedrullningsknappen. |

### Exempel

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
            // Initiera en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ComboBox ActiveX-kontroll i kalkylbladet
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Ställ in egenskaper för ComboBox ActiveX-kontrollen
            comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus; // Show drop button when the control has focus
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.IsEditable = true;

            // Lägg till några objekt i ComboBoxen
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Spara arbetsboken
            workbook.Save("ShowDropButtonTypeExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


