---
title: "CellsColor.IsShapeColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsColor özelliği. Hücreye veya şekle uygulanacak rengi alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/cellscolor/isshapecolor/
---
## CellsColor.IsShapeColor property

Hücreye veya şekle uygulanacak rengi alır ve ayarlar.

```csharp
public bool IsShapeColor { get; set; }
```

### Açıklamalar

Hücre ve şeklin renk ifadesi farklıdır. Örneğin, aynı ton değerine sahip tema rengi hücrede ve şekilde aynı olmayacaktır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyIsShapeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir CellsColor örneği oluştur ve IsShapeColor'ı ayarla
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.IsShapeColor = true;
            cellsColor.Color = Color.Green;

            // Rengi bir şekle uygula
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = cellsColor.Color;  // Use the Color property instead of CellsColor directly

            // Çalışma kitabını kaydedin
            workbook.Save("CellsColorIsShapeColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


