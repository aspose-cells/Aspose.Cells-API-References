---
title: "ComboBox.Shadow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ComboBox. Indique si le combobox possède un ombrage 3D"
type: docs
url: /fr/net/aspose.cells.drawing/combobox/shadow/
---
## ComboBox.Shadow property

Indique si la zone de liste déroulante possède un ombrage 3D.

```csharp
public bool Shadow { get; set; }
```

### Exemples

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

### Voir aussi

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


