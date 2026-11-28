---
title: "Enum EquationFractionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Equations.EquationFractionType enum. Bu, kesir çubuğunun görüntüleme stilini belirtir."
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationfractiontype/
---
## EquationFractionType enumeration

Bu, kesir çubuğunun görüntü stilini belirtir.

```csharp
public enum EquationFractionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Bar | `0` | Bu, payın üstte ve paydanın altta olduğu, ortada bir çubukla ayrıldığı anlamına gelir. |
| NoBar | `1` | Bu, payın üstte ve paydanın altta olduğu, ortada bir çubukla ayrılmadığı anlamına gelir. |
| Linear | `2` | Bu, payın solda ve paydanın sağda olduğu, arada '/' ile ayrıldığı anlamına gelir. |
| Skewed | `3` | Bu, payın üst sol köşede ve paydanın alt sağ köşede olduğu, '/' ile ayrıldığı anlamına gelir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationFractionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Denklem şekli ekle
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Matematik düğümünü alın ve kesir ekleyin.
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Payı ekle
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "A";

            // Payda ekle
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "B";

            // Kaydet ve doğrula
            workbook.Save("EquationFractionTypeDemo.xlsx");
            
            Console.WriteLine("Equation with skewed fraction created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


