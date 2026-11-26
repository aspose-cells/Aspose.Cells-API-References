---
title: "Перечисление EquationDelimiterShapeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType перечисление. Это указывает форму разделителей в объекте разделителя."
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationdelimitershapetype/
---
## EquationDelimiterShapeType enumeration

Это определяет форму разделителей в объекте разделителя.

```csharp
public enum EquationDelimiterShapeType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Centered | `0` | Разделитель центрируется по всей высоте своего содержимого. |
| Match | `1` | Разделитель изменяется, чтобы точно соответствовать высоте их содержимого. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationDelimiterShapeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить форму уравнения
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Получить узел уравнения
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Создать узел разделителя с типом формы Match
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "{";
            delimiterNode.EndChar = "}";
            
            // Добавить содержимое внутри разделителя
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";
            
            // Сохраните книгу
            workbook.Save("EquationDelimiterShapeTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


