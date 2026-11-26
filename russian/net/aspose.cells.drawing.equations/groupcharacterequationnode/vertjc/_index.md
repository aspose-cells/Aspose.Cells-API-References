---
title: "GroupCharacterEquationNode.VertJc"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GroupCharacterEquationNode. Этот атрибут в сочетании с pos из groupChrPr определяет вертикальное расположение объекта groupChr. Где pos указывает позицию группирующего символа, vertJc определяет выравнивание объекта относительно базовой линии."
type: docs
url: /ru/net/aspose.cells.drawing.equations/groupcharacterequationnode/vertjc/
---
## GroupCharacterEquationNode.VertJc property

Этот атрибут в сочетании с pos из groupChrPr определяет вертикальное расположение объекта groupChr. Где pos указывает позицию группирующего символа, vertJc задает выравнивание объекта относительно базовой линии.

```csharp
public EquationCharacterPositionType VertJc { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class GroupCharacterEquationNodePropertyVertJcDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму текстового поля для размещения уравнения
            var shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            
            // Создать экземпляр GroupCharacterEquationNode
            var equationNode = (GroupCharacterEquationNode)shape.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            
            try
            {
                // Установить начальные свойства узла уравнения
                equationNode.GroupChr = "⏟";
                equationNode.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
                equationNode.Position = EquationCharacterPositionType.Bottom;
                
                // Продемонстрировать свойство VertJc (чтение и запись)
                Console.WriteLine("Initial VertJc value: " + equationNode.VertJc);
                
                // Изменить значение VertJc
                equationNode.VertJc = EquationCharacterPositionType.Top;
                Console.WriteLine("Modified VertJc value: " + equationNode.VertJc);
                
                // Сохраните книгу
                workbook.Save("VertJcDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


