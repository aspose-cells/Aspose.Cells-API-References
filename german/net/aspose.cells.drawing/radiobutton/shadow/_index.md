---
title: "RadioButton.Shadow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RadioButton-Eigenschaft. Gibt an, ob das ComboBox 3D-Schattierung hat"
type: docs
url: /de/net/aspose.cells.drawing/radiobutton/shadow/
---
## RadioButton.Shadow property

Gibt an, ob die ComboBox 3‑D‑Schattierung hat.

```csharp
public bool Shadow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RadioButtonPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            RadioButton radio = worksheet.Shapes.AddRadioButton(0, 0, 100, 50, 0, 0);
            radio.Text = "Option 1";
            radio.Shadow = true;

            workbook.Save("RadioButtonShadowDemo.xlsx", SaveFormat.Xlsx);

            Workbook loadedWorkbook = new Workbook("RadioButtonShadowDemo.xlsx");
            RadioButton loadedRadio = (RadioButton)loadedWorkbook.Worksheets[0].Shapes[0];

            Console.WriteLine("Shadow visible: " + loadedRadio.Shadow);
        }
    }
}
```

### Siehe auch

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


