---
title: "BarEquationNode.BarPosition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BarEquationNode. Этот атрибут указывает позицию полосы в объекте bar"
type: docs
url: /ru/net/aspose.cells.drawing.equations/barequationnode/barposition/
---
## BarEquationNode.BarPosition property

Этот атрибут указывает положение линии в объекте bar

```csharp
public EquationCharacterPositionType BarPosition { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class BarEquationNodePropertyBarPositionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте форму уравнения на первый лист
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Получить узел уравнения
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Создать узел уравнения бар
            BarEquationNode barNode = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
            
            // Установить позицию полосы в Top
            barNode.BarPosition = EquationCharacterPositionType.Top;

            // Добавить базовое содержимое для полосы
            EquationNode baseNode = barNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // Сохраните книгу
            workbook.Save("BarEquationDemo.xlsx");

            // Проверьте сохранённый файл
            Workbook verifyWorkbook = new Workbook("BarEquationDemo.xlsx");
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            BarEquationNode verifyBarNode = (BarEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Bar Position: " + verifyBarNode.BarPosition);
            Console.WriteLine("Base Content: " + ((TextRunEquationNode)verifyBarNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### См. также

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


