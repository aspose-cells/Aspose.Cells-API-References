---
title: "MatrixEquationNode.IsHidePlaceholder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MatrixEquationNode. Этот атрибут задает свойство Hide Placeholders для матрицы. Когда это свойство включено, заполнители не отображаются в матрице. По умолчанию заполнители отображаются, чтобы сделать видимыми места, куда можно вставить текст."
type: docs
url: /ru/net/aspose.cells.drawing.equations/matrixequationnode/ishideplaceholder/
---
## MatrixEquationNode.IsHidePlaceholder property

Этот атрибут задает свойство Hide Placeholders для матрицы. Когда это свойство включено, заполнители не отображаются в матрице. По умолчанию заполнители отображаются, делая видимыми места, куда можно вставить текст.

```csharp
public bool IsHidePlaceholder { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class MatrixEquationNodePropertyIsHidePlaceholderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить форму уравнения
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Получите математический узел и добавьте матрицу
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Установить свойства матрицы
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true; // Demonstrate IsHidePlaceholder property

            // Добавьте 2x2 матрицу с единицами на диагонали
            for (int row = 0; row < 2; row++)
            {
                EquationNode matrixRow = matrixNode.AddChild(EquationNodeType.MatrixRow);
                for (int col = 0; col < 2; col++)
                {
                    EquationNode baseNode = matrixRow.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (row == col) ? "1" : "0";
                }
            }

            // Сохранить и проверить
            string outputPath = "MatrixEquationWithHiddenPlaceholder.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation created with IsHidePlaceholder=true. File saved to: " + outputPath);
        }
    }
}
```

### См. также

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


