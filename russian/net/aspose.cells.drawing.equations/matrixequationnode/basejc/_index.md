---
title: "MatrixEquationNode.BaseJc"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MatrixEquationNode. Этот атрибут задает выравнивание матрицы. Текст за пределами матрицы может быть выровнен по нижнему, верхнему или центральному краю функции матрицы. По умолчанию матрица использует центральное выравнивание."
type: docs
url: /ru/net/aspose.cells.drawing.equations/matrixequationnode/basejc/
---
## MatrixEquationNode.BaseJc property

Этот атрибут задает выравнивание матрицы. Текст за пределами матрицы может быть выровнен по нижнему, верхнему краю или по центру функции матрицы. По умолчанию матрица выравнивается по центру.

```csharp
public EquationVerticalJustificationType BaseJc { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class MatrixEquationNodePropertyBaseJcDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте форму уравнения на первый лист
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Получить абзац уравнения и добавить узел матрицы
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Установите свойства матрицы, включая BaseJc
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // Добавьте содержимое 2x2 матрицы (единичная матрица)
            for (int row = 0; row < 2; row++)
            {
                EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
                
                for (int col = 0; col < 2; col++)
                {
                    EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (row == col) ? "1" : "0";
                }
            }

            // Сохраните книгу
            string outputPath = "MatrixEquationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation with BaseJc property demo completed.");
        }
    }
}
```

### См. также

* enum [EquationVerticalJustificationType](../../equationverticaljustificationtype/)
* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


