---
title: "ComboBox.Shadow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ComboBox. تشير إلى ما إذا كان combobox يحتوي على تظليل ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.drawing/combobox/shadow/
---
## ComboBox.Shadow property

يشير إلى ما إذا كان صندوق الجمع يحتوي على تظليل ثلاثي الأبعاد.

```csharp
public bool Shadow { get; set; }
```

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            ComboBox sourceCombo = sheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 20);
            sourceCombo.Shadow = true;
            sourceCombo.InputRange = "A1:A3";
            sourceCombo.LinkedCell = "B1";

            ComboBox destCombo = sheet.Shapes.AddComboBox(4, 0, 4, 0, 100, 20);
            destCombo.Shadow = false;
            destCombo.InputRange = "A1:A3";
            destCombo.LinkedCell = "B2";

            workbook.Save("BeforeShadowCopy.xlsx");
            destCombo.Shadow = sourceCombo.Shadow;
            workbook.Save("AfterShadowCopy.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


