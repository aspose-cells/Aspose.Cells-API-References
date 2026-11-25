---
title: "ComboBox.Shadow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ComboBox. Indica se il combobox ha ombreggiatura 3D"
type: docs
url: /it/net/aspose.cells.drawing/combobox/shadow/
---
## ComboBox.Shadow property

Indica se la combobox ha ombreggiatura 3D.

```csharp
public bool Shadow { get; set; }
```

### Esempi

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

### Vedi anche

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


