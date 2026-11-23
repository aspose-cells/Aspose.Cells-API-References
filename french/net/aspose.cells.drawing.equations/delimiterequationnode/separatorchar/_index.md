---
title: "DelimiterEquationNode.SeparatorChar"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DelimiterEquationNode. Caractère séparateur du délimiteur"
type: docs
url: /fr/net/aspose.cells.drawing.equations/delimiterequationnode/separatorchar/
---
## DelimiterEquationNode.SeparatorChar property

Caractère séparateur du délimiteur.

```csharp
public string SeparatorChar { get; set; }
```

### Remarques

Il convient de noter que cette propriété n'accepte qu'un seul caractère, et si plusieurs caractères sont fournis, seul le premier caractère est accepté.

### Exemples

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

### Voir aussi

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


