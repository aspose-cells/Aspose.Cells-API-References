---
title: "EquationComponentNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод EquationComponentNode. Определяет, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationcomponentnode/equals/
---
## EquationComponentNode.Equals method

Определить, равен ли текущий узел уравнения указанному узлу

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object | Указанный узел |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationComponentNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //тест get mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            //тест insert Fraction
            FractionEquationNode node = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            node.FractionType = EquationFractionType.Skewed;

            string str1 = "A";
            EquationComponentNode numerator = (EquationComponentNode)node.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode TR = (TextRunEquationNode)(numerator.AddChild(EquationNodeType.Text));
            TR.Text = str1;

            string str2 = "B";
            EquationComponentNode denominator = (EquationComponentNode)node.AddChild(EquationNodeType.Denominator);
            TR = (TextRunEquationNode)(denominator.AddChild(EquationNodeType.Text));
            TR.Text = str2;

            // Сравните узлы, используя метод Equals
            bool areEqual = numerator?.Equals((object)denominator) ?? false;

            // Отобразите результат сравнения
            Console.WriteLine($"Nodes are equal: {areEqual}");
            workbook.Save("EquationComponentNodeMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### См. также

* class [EquationComponentNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


