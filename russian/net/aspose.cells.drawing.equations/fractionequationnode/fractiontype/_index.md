---
title: "FractionEquationNode.FractionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FractionEquationNode. Указывает тип дроби, по умолчанию Bar"
type: docs
url: /ru/net/aspose.cells.drawing.equations/fractionequationnode/fractiontype/
---
## FractionEquationNode.FractionType property

Это указывает тип дроби; по умолчанию — 'Bar'.

```csharp
public EquationFractionType FractionType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class FractionEquationNodePropertyFractionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить форму уравнения
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Получить математический узел
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Создать узел дроби
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Добавить числитель
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "A";

            // Добавить знаменатель
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "B";

            // Сохранить и проверить
            string outputPath = "FractionEquationDemo.xlsx";
            workbook.Save(outputPath);

            // Перезагрузить для проверки
            Workbook verifyWorkbook = new Workbook(outputPath);
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            FractionEquationNode verifyFraction = (FractionEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Fraction Type: " + verifyFraction.FractionType);
            Console.WriteLine("Numerator: " + ((TextRunEquationNode)verifyFraction.GetChild(0).GetChild(0)).Text);
            Console.WriteLine("Denominator: " + ((TextRunEquationNode)verifyFraction.GetChild(1).GetChild(0)).Text);
        }
    }
}
```

### См. также

* enum [EquationFractionType](../../equationfractiontype/)
* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


