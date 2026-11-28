---
title: "DelimiterEquationNode.EndChar"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DelimiterEquationNode özelliği. Sınırlayıcı bitiş karakteri"
type: docs
url: /tr/net/aspose.cells.drawing.equations/delimiterequationnode/endchar/
---
## DelimiterEquationNode.EndChar property

Sınırlayıcı bitiş karakteri.

```csharp
public string EndChar { get; set; }
```

### Açıklamalar

Bu özelliğin yalnızca bir karakter kabul ettiğini ve birden fazla karakter gönderildiğinde sadece ilk karakterin kabul edildiğini belirtmek gerekir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyEndCharDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Denklem düğümünü al
            var mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Özel bir bitiş karakteriyle bir sınırlayıcı düğüm oluştur
            var delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]"; // Demonstrating EndChar property
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;

            // Sınırlayıcının içine içerik ekle
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";

            // Kaydet ve doğrula
            string outputPath = "DelimiterEquationDemo.xlsx";
            workbook.Save(outputPath);

            // Kaydedilen dosyayı doğrula
            Workbook verifyWorkbook = new Workbook(outputPath);
            var verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            var verifyNode = (DelimiterEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);

            Console.WriteLine("BeginChar: " + verifyNode.BeginChar);
            Console.WriteLine("EndChar: " + verifyNode.EndChar); // Output the EndChar value
        }
    }
}
```

### Ayrıca Bakınız

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


