---
title: "DelimiterEquationNode.SeparatorChar"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DelimiterEquationNode özelliği. Ayraç ayırıcı karakteri"
type: docs
url: /tr/net/aspose.cells.drawing.equations/delimiterequationnode/separatorchar/
---
## DelimiterEquationNode.SeparatorChar property

Sınırlayıcı ayırıcı karakteri.

```csharp
public string SeparatorChar { get; set; }
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
    public class DelimiterEquationNodePropertySeparatorCharDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            TextBox textBox = worksheet.Shapes.AddEquation(0, 0, 0, 0, 100, 200);
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            DelimiterEquationNode delimiter = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiter.BeginChar = "{";
            delimiter.EndChar = "}";
            delimiter.SeparatorChar = "|";
            delimiter.DelimiterShape = EquationDelimiterShapeType.Match;
            
            string filePath = "DelimiterEquationExample.xlsx";
            workbook.Save(filePath);
            
            Workbook loadedWorkbook = new Workbook(filePath);
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            DelimiterEquationNode loadedDelimiter = (DelimiterEquationNode)loadedTextBox.GetEquationParagraph()
                .GetChild(0).GetChild(0);
            
            Console.WriteLine("SeparatorChar: " + loadedDelimiter.SeparatorChar);
        }
    }
}
```

### Ayrıca Bakınız

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


