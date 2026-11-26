---
title: "EquationNode.CreateNode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод EquationNode. Создаёт узел указанного типа"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationnode/createnode/
---
## EquationNode.CreateNode method

Создать узел указанного типа.

```csharp
public static EquationNode CreateNode(EquationNodeType equationType, Workbook workbook, 
    EquationNode parent)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| equationType | EquationNodeType | Типы узлов уравнения |
| рабочая книга | Рабочая книга | Объект книги, связанный с уравнением |
| родитель | EquationNode | Родительский узел, в котором находится этот узел |

### Возвращаемое значение

Если указанный тип существует, возвращается соответствующий узел; если тип не существует, возвращается узел неизвестного типа.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodCreateNodeWithEquationNodeTypeWorkbookEquatiDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму уравнения
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Создайте родительский узел (дробь)
                var fractionNode = EquationNode.CreateNode(EquationNodeType.Fraction, workbook, null);
                
                // Создайте узлы числителя и знаменателя
                var numeratorNode = EquationNode.CreateNode(EquationNodeType.Numerator, workbook, fractionNode);
                var numeratorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, numeratorNode) as TextRunEquationNode;
                numeratorText.Text = "a + b";
                
                var denominatorNode = EquationNode.CreateNode(EquationNodeType.Denominator, workbook, fractionNode);
                var denominatorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, denominatorNode) as TextRunEquationNode;
                denominatorText.Text = "c";

                // Добавьте созданную дробь к основному уравнению
                equationNode.AddChild(fractionNode);

                Console.WriteLine("Equation created successfully using CreateNode method");
                
                // Отобразите уравнение в ячейке
                worksheet.Cells["A1"].PutValue("Equation Output:");
                worksheet.Cells["B1"].PutValue(equationNode.ToLaTeX());
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CreateNode method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("EquationNodeCreateNodeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [EquationNodeType](../../equationnodetype/)
* class [Workbook](../../../aspose.cells/workbook/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


