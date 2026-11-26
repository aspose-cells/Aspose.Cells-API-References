---
title: "DelimiterEquationNode.BeginChar"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DelimiterEquationNode. Символ начала разделителя"
type: docs
url: /ru/net/aspose.cells.drawing.equations/delimiterequationnode/beginchar/
---
## DelimiterEquationNode.BeginChar property

Символ начала разделителя.

```csharp
public string BeginChar { get; set; }
```

### Примечания

Следует отметить, что это свойство принимает только один символ, и если передано несколько символов, принимается только первый.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyBeginCharDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить уравнение на первый лист
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
            
            // Получить корневой узел уравнения
            var mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Добавить узел разделителя с пользовательскими символами начала/завершения
            var delimiterNode = mathNode.AddChild(EquationNodeType.Delimiter) as DelimiterEquationNode;
            delimiterNode.BeginChar = "#";
            delimiterNode.EndChar = "*";
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            
            // Добавить содержимое внутри разделителя
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Sample Content";
            
            // Сохраните книгу
            string outputPath = "DelimiterEquationDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Workbook saved with custom delimiter equation. BeginChar: " + delimiterNode.BeginChar);
        }
    }
}
```

### См. также

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


