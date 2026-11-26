---
title: "TextRunEquationNode.Text"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextRunEquationNode. Установите содержимое текстового узла. Обычно объект узла соответствует одному символу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/textrunequationnode/text/
---
## TextRunEquationNode.Text property

Установить содержимое текстового узла (обычно объект узла создаётся для каждого символа).

```csharp
public string Text { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class TextRunEquationNodePropertyTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте форму уравнения на первый лист
            TextBox textBox = (TextBox)workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Получить корневой узел уравнения
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Создать дробное уравнение
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Добавить числитель с текстом \"X\"
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "X";

            // Добавить знаменатель с текстом \"Y\"
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "Y";

            // Сохраните книгу
            workbook.Save("TextRunEquationNodeDemo.xlsx");

            // Проверьте сохранённый файл, загрузив его обратно
            Workbook loadedWorkbook = new Workbook("TextRunEquationNodeDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Получить доступ к свойствам текста для демонстрации функциональности
            TextRunEquationNode loadedNumeratorText = (TextRunEquationNode)((FractionEquationNode)loadedTextBox
                .GetEquationParagraph()
                .GetChild(0)
                .GetChild(0))
                .GetChild(0)
                .GetChild(0);

            Console.WriteLine("Numerator text: " + loadedNumeratorText.Text);
        }
    }
}
```

### См. также

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


