---
title: "RadioButton.Shadow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RadioButton. Indica se il combobox ha ombreggiatura 3D"
type: docs
url: /it/net/aspose.cells.drawing/radiobutton/shadow/
---
## RadioButton.Shadow property

Indica se la combobox ha ombreggiatura 3D.

```csharp
public bool Shadow { get; set; }
```

### Esempi

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

### Vedi anche

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


