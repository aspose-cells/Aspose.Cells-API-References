---
title: "Shape.LineFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Şekil özelliği. Belirtilen şekil için satır biçimlendirme özelliklerini içeren bir MsoLineFormat nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/shape/lineformat/
---
## Shape.LineFormat property

Belirtilen şekil için satır biçimlendirme özelliklerini içeren bir MsoLineFormat nesnesi döndürür.

```csharp
[Obsolete("Use Shape.Line property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoLineFormat LineFormat { get; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Line özelliğini kullanın. Bu özellik Temmuz 2016'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına bir dikdörtgen şekli ekle.
            Worksheet worksheet = workbook.Worksheets[0];
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(3, 0, 2, 0, 70, 130);
            
            // Şekil özelliklerini ayarla
            rectangle.Placement = PlacementType.FreeFloating;
            rectangle.Fill.FillType = FillType.Solid;
            rectangle.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            
            // LineFormat kullanımını göster
            rectangle.LineFormat.Weight = 3; // Set line weight
            rectangle.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            rectangle.Line.SolidFill.Color = System.Drawing.Color.DarkBlue; // Correct way to set line color
            
            // Çalışma kitabını kaydedin
            workbook.Save("ShapeLineFormatDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoLineFormat](../../msolineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


