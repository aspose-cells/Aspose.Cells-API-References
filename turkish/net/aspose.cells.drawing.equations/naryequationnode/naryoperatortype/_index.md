---
title: "NaryEquationNode.NaryOperatorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "NaryEquationNode özelliği. bir nary operatör. örn."
type: docs
url: /tr/net/aspose.cells.drawing.equations/naryequationnode/naryoperatortype/
---
## NaryEquationNode.NaryOperatorType property

n-ary bir operatör. örn. "∑"

```csharp
public EquationMathematicalOperatorType NaryOperatorType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyNaryOperatorTypeDemo
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

            // NaryOperatorType özelliğine erişmek için NaryEquationNode tipine dönüştürün
            var naryEquationNode = (NaryEquationNode)naryNode;

            // Mevcut NaryOperatorType değerini gösterin (varsayılan değer)
            Console.WriteLine("Current NaryOperatorType: " + naryEquationNode.NaryOperatorType);

            // Toplam operatörüne (∑) ayarlayın
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Operatörü göstermek için taban (operand) ve limitleri ekleyin
            var baseNode = naryEquationNode.AddChild(EquationNodeType.Base);
            var textNode1 = baseNode.AddChild(EquationNodeType.Text);
            textNode1.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var limitNode = naryEquationNode.AddChild(EquationNodeType.Limit);
            var textNode2 = limitNode.AddChild(EquationNodeType.Text);
            textNode2.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var textNode3 = baseNode.AddChild(EquationNodeType.Text);
            textNode3.ToLaTeX(); // This would be where you'd set the text content if the API allowed

            // Operatörü içeriğiyle birlikte büyüyecek şekilde ayarlayın
            naryEquationNode.NaryGrow = true;

            // Ürün operatörüne (∏) değiştirin ve farkı gösterin
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;

            // Çalışma kitabını kaydedin
            workbook.Save("NaryOperatorTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [EquationMathematicalOperatorType](../../equationmathematicaloperatortype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


