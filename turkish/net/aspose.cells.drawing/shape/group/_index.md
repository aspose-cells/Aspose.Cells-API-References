---
title: "Shape.Group"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Bu şekli içeren grup şekli alır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/group/
---
## Shape.Group property

Bu şekli içeren grup şeklini alır.

```csharp
public GroupShape Group { get; }
```

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGroupDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // İki örnek şekil oluşturun
            Shape shape1 = sheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 0);
            Shape shape2 = sheet.Shapes.AddOval(0, 100, 100, 100, 100, 0);

            // Şekilleri Shape dizi parametresi kullanarak gruplayın
            GroupShape group = sheet.Shapes.Group(new Shape[] { shape1, shape2 });

            // Alt şeklin Group özelliği aracılığıyla gruba erişin
            GroupShape retrievedGroup = shape1.Group;
            
            // Group özelliğinin kullanımını gösterin
            retrievedGroup.Name = "MyShapeGroup";
            retrievedGroup.Placement = PlacementType.FreeFloating;

            workbook.Save("GroupShapeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


