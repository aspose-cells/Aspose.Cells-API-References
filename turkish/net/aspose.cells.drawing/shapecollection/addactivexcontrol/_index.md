---
title: "ShapeCollection.AddActiveXControl"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Bir Activex Kontrolü oluşturur"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addactivexcontrol/
---
## ShapeCollection.AddActiveXControl method

Bir Activex Kontrolü oluşturur.

```csharp
public Shape AddActiveXControl(ControlType type, int topRow, int top, int leftColumn, int left, 
    int width, int height)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | ControlType | Kontrolün türü. |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | Shape'in sol satırından dikey ofsetini piksel biriminde temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | Shape'in sol sütunundan yatay ofsetini piksel biriminde temsil eder. |
| yükseklik | Int32 | Shape'in yüksekliğini piksel biriminde temsil eder. |
| genişlik | Int32 | Shape'in genişliğini piksel biriminde temsil eder. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddActiveXControlWithControlTypeInt32Int32Int32Int3Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            Shape activeXControl = shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 
                1,  // upperLeftRow
                0,  // top
                1,  // upperLeftColumn
                0,  // left
                100,  // width
                50   // height
            );

            workbook.Save("AddActiveXControlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* enum [ControlType](../../../aspose.cells.drawing.activexcontrols/controltype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


