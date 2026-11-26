---
title: "AccentEquationNode.AccentCharacter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AccentEquationNode. Этот атрибут указывает тип комбинирующего диакритического знака, присоединяемого к основе функции акцента. Символ акцента по умолчанию — U0302. Настоятельно рекомендуется использовать атрибут AccentType для установки символа акцента. Используйте эту настройку свойства, если вы не можете найти нужный символ в известном типе."
type: docs
url: /ru/net/aspose.cells.drawing.equations/accentequationnode/accentcharacter/
---
## AccentEquationNode.AccentCharacter property

Этот атрибут указывает тип комбинирующего диакритического знака, присоединяемого к основе функции надстрочного знака. Символ надстрочного знака по умолчанию — U+0302. Настоятельно рекомендуется использовать атрибут AccentType для установки символа надстрочного знака. Используйте эту настройку свойства, если не можете найти нужный символ в известном типе.

```csharp
public string AccentCharacter { get; set; }
```

### Примечания

Следует отметить, что это свойство принимает только один символ, и если передано несколько символов, принимается только первый.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class AccentEquationNodePropertyAccentCharacterDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте форму уравнения на первый лист
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Получите узел уравнения и добавьте узел акцента
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            
            // Установите символ акцента (в данном случае циркумфлекс)
            accentNode.AccentCharacter = "\u0302";

            // Добавьте базовый текст для акцента
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "x";

            // Сохраните книгу
            workbook.Save("AccentEquationDemo.xlsx");

            // Проверьте сохранённый файл, загрузив его обратно
            Workbook loadedWorkbook = new Workbook("AccentEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            AccentEquationNode loadedAccentNode = (AccentEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            // Выведите символ акцента, чтобы продемонстрировать свойство
            Console.WriteLine("Accent Character: " + loadedAccentNode.AccentCharacter);
        }
    }
}
```

### См. также

* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


