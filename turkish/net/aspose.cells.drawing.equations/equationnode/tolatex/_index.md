---
title: "EquationNode.ToLaTeX"
second_title: "Aspose.Cells için .NET API Referansı"
description: "EquationNode yöntemi. Bu denklemi LaTeX ifadesine dönüştür"
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationnode/tolatex/
---
## EquationNode.ToLaTeX method

Bu equtation'ı LaTeX ifadesine dönüştür.

```csharp
public string ToLaTeX()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodToLaTeXDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Denklemi tutacak bir şekil oluştur
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);

            // Denklem düğümünü al
            var equationNode = shape.GetEquationParagraph();

            // Basit bir kesir denklemi oluştur
            var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            numeratorText.Text = "1";
            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            denominatorText.Text = "2";

            try
            {
                // ToLaTeX yöntemini çağır
                string latexExpression = equationNode.ToLaTeX();
                
                // Sonucu göster
                Console.WriteLine("LaTeX expression: " + latexExpression);
                
                // LaTeX çıktısını bir hücreye ekle
                worksheet.Cells["A1"].PutValue("LaTeX Output:");
                worksheet.Cells["B1"].PutValue(latexExpression);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToLaTeX method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("EquationToLaTeXDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


