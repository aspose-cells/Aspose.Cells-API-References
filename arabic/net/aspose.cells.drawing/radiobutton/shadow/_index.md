---
title: "RadioButton.Shadow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RadioButton. تشير إلى ما إذا كان RadioButton يحتوي على تظليل ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.drawing/radiobutton/shadow/
---
## RadioButton.Shadow property

يشير إلى ما إذا كان صندوق الجمع يحتوي على تظليل ثلاثي الأبعاد.

```csharp
public bool Shadow { get; set; }
```

### أمثلة

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

### انظر أيضًا

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


