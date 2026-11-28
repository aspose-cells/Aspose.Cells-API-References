---
title: "EquationNodeParagraph.Justification"
second_title: "Aspose.Cells için .NET API Referansı"
description: "EquationNodeParagraph özelliği. Bu, aynı paragrafta yan yana gelen bir dizi denklemi içeren matematik paragrafının hizalamasını belirtir. Bir matematik paragrafı Sol Hizalı, Sağ Hizalı, Ortalanmış veya Grup Olarak Ortalanmış olabilir. Varsayılan olarak matematik paragrafı Grup Olarak Ortalanmıştır. Bu, denklemlerin birbirlerine göre hizalanabileceği ancak tüm denklemler grubunun bütün olarak ortalandığı anlamına gelir."
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationnodeparagraph/justification/
---
## EquationNodeParagraph.Justification property

Bu, matematik paragrafının hizalamasını belirtir (aynı paragrafta yan yana bulunan bir dizi denklem). Bir matematik paragrafı Sol Hizalı, Sağ Hizalı, Ortalanmış veya Grup Olarak Ortalanmış olabilir. Varsayılan olarak, matematik paragrafı Grup Olarak Ortalanmıştır. Bu, denklemlerin birbirlerine göre hizalanabileceği, ancak tüm denklem grubunun bütün olarak ortalandığı anlamına gelir.

```csharp
public EquationHorizontalJustificationType Justification { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeParagraphPropertyJustificationDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Denklemi tutacak bir şekil oluştur
            var shape = worksheet.Shapes.AddTextBox(0, 0, 200, 50, 200, 50);

            // Denklem paragrafını al
            var equationParagraph = shape.GetEquationParagraph() as EquationNodeParagraph;

            // Mevcut hizalama değerini göster
            Console.WriteLine("Current Justification value: " + equationParagraph.Justification);

            // Farklı hizalama değerleri ayarlayın ve etkileri gözlemleyin
            equationParagraph.Justification = EquationHorizontalJustificationType.Left;
            Console.WriteLine("Set to Left justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Center;
            Console.WriteLine("Set to Center justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.CenterGroup;
            Console.WriteLine("Set to CenterGroup justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Right;
            Console.WriteLine("Set to Right justification");

            // Çalışma kitabını kaydedin
            workbook.Save("EquationJustificationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [EquationHorizontalJustificationType](../../equationhorizontaljustificationtype/)
* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


