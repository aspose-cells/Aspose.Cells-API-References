---
title: "RadioButton.Shadow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RadioButton. Indica si el combobox tiene sombreado 3D"
type: docs
url: /es/net/aspose.cells.drawing/radiobutton/shadow/
---
## RadioButton.Shadow property

Indica si el cuadro combinado tiene sombreado 3D.

```csharp
public bool Shadow { get; set; }
```

### Ejemplos

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

### Ver también

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


