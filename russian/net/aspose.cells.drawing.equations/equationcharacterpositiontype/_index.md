---
title: "Перечисление EquationCharacterPositionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.Equations.EquationCharacterPositionType enum. Указывает положение конкретного подобъекта внутри его родителя"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationcharacterpositiontype/
---
## EquationCharacterPositionType enumeration

Указывает позицию конкретного подобъекта внутри его родителя

```csharp
public enum EquationCharacterPositionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Top | `0` | В верхней части родительского объекта |
| Bottom | `1` | В нижней части родительского объекта |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationCharacterPositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить форму уравнения
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Получить узел уравнения и добавить черту с верхней позицией
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            BarEquationNode barNode = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
            barNode.BarPosition = EquationCharacterPositionType.Top;
            
            // Добавить базовый текст
            EquationNode baseNode = barNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";
            
            // Сохранить и проверить
            string outputFile = "EquationCharacterPositionTypeDemo.xlsx";
            workbook.Save(outputFile);
            
            // Перезагрузить и проверить
            Workbook loadedWorkbook = new Workbook(outputFile);
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            BarEquationNode loadedBarNode = (BarEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Bar Position: " + loadedBarNode.BarPosition);
            Console.WriteLine("Text Content: " + ((TextRunEquationNode)loadedBarNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


