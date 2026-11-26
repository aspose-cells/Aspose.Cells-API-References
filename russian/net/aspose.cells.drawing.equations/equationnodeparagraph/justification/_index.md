---
title: "EquationNodeParagraph.Justification"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство EquationNodeParagraph. Указывает выравнивание математического абзаца — серии смежных уравнений в одном абзаце. Математический абзац может быть выровнен по левому краю, по правому краю, по центру или центрирован как группа. По умолчанию математический абзац центрирован как группа. Это означает, что уравнения могут быть выровнены относительно друг друга, но вся группа уравнений центрирована в целом."
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationnodeparagraph/justification/
---
## EquationNodeParagraph.Justification property

Это указывает выравнивание математического абзаца (серии соседних уравнений в одном абзаце). Математический абзац может быть выровнен по левому краю, по правому краю, по центру или центрирован как группа. По умолчанию математический абзац центрирован как группа. Это означает, что уравнения могут быть выровнены относительно друг друга, но вся группа уравнений центрирована в целом.

```csharp
public EquationHorizontalJustificationType Justification { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeParagraphPropertyJustificationDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму для размещения уравнения
            var shape = worksheet.Shapes.AddTextBox(0, 0, 200, 50, 200, 50);

            // Получить абзац уравнения
            var equationParagraph = shape.GetEquationParagraph() as EquationNodeParagraph;

            // Отобразите текущее значение выравнивания
            Console.WriteLine("Current Justification value: " + equationParagraph.Justification);

            // Установите разные значения выравнивания и наблюдайте эффекты
            equationParagraph.Justification = EquationHorizontalJustificationType.Left;
            Console.WriteLine("Set to Left justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Center;
            Console.WriteLine("Set to Center justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.CenterGroup;
            Console.WriteLine("Set to CenterGroup justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Right;
            Console.WriteLine("Set to Right justification");

            // Сохраните книгу
            workbook.Save("EquationJustificationDemo.xlsx");
        }
    }
}
```

### См. также

* enum [EquationHorizontalJustificationType](../../equationhorizontaljustificationtype/)
* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


