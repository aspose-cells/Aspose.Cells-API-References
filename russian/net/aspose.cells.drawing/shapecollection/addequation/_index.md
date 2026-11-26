---
title: "ShapeCollection.AddEquation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ShapeCollection метод. Добавляет объект уравнения на лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addequation/
---
## ShapeCollection.AddEquation method

Добавляет объект уравнения на лист.

```csharp
public TextBox AddEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс верхней строки. |
| верх | Int32 | Вертикальное смещение его верхней строки в пикселях. |
| leftColumn | Int32 | Индекс левой колонки. |
| влево | Int32 | Горизонтальное смещение от её левой колонки, в пикселях. |
| высота | Int32 | Высота уравнения, в пикселях. |
| ширина | Int32 | Ширина уравнения, в пикселях. |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddEquationWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            FractionEquationNode fraction = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fraction.FractionType = EquationFractionType.Skewed;

            EquationComponentNode numerator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numText.Text = "A";

            EquationComponentNode denominator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denText.Text = "B";

            workbook.Save("ShapeEquationDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


