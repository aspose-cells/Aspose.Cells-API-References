---
title: "NaryEquationNode.LimitLocation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "NaryEquationNode özelliği. Bu öznitelik, nary operatörlerde limitlerin konumunu belirtir. Limitler, nary operatörün üstünde ve altında ortalanmış ya da operatörün hemen sağ tarafına konumlandırılmış olabilir."
type: docs
url: /tr/net/aspose.cells.drawing.equations/naryequationnode/limitlocation/
---
## NaryEquationNode.LimitLocation property

Bu öznitelik, n-ary operatörlerde limitlerin konumunu belirtir. Limitler, n-ary operatörün üstünde ve altında ortalanmış ya da operatörün hemen sağında konumlandırılmış olabilir.

```csharp
public EquationLimitLocationType LimitLocation { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyLimitLocationDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Denklemi tutacak bir şekil oluştur
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // Denkleme erişin ve bir nary operatör düğümü ekleyin
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // LimitLocation özelliğine erişmek için NaryEquationNode tipine dönüştür
            var naryEquationNode = (NaryEquationNode)naryNode;

            try
            {
                // Mevcut LimitLocation'ı göster (varsayılan değer)
                Console.WriteLine("Default LimitLocation: " + naryEquationNode.LimitLocation);

                // LimitLocation'ı SubSup olarak ayarla (limitler sağ tarafta)
                naryEquationNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("After setting to SubSup: " + naryEquationNode.LimitLocation);

                // UndOvr olarak geri değiştir (ortalanmış limitler)
                naryEquationNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("After setting to UndOvr: " + naryEquationNode.LimitLocation);

                // Çalışma kitabını kaydedin
                workbook.Save("LimitLocationDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [EquationLimitLocationType](../../equationlimitlocationtype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


