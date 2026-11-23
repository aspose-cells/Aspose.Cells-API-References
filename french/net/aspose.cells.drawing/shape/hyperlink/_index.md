---
title: "Shape.Hyperlink"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient le lien hypertexte de la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/hyperlink/
---
## Shape.Hyperlink property

Obtient le lien hypertexte de la forme.

```csharp
public Hyperlink Hyperlink { get; }
```

### Exemples

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapePropertyHyperlinkDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.Shape shape = sheet.Shapes.AddRectangle(0, 0, 10, 10, 100, 150);
            Hyperlink hyperlink = shape.Hyperlink;
            hyperlink.Address = "https://www.aspose.com";
            hyperlink.ScreenTip = "Click to open Aspose website";

            workbook.Save("ShapeHyperlinkDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Hyperlink](../../../aspose.cells/hyperlink/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


