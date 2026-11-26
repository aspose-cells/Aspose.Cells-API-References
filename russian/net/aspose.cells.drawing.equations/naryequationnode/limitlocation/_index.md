---
title: "NaryEquationNode.LimitLocation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство NaryEquationNode. Этот атрибут указывает расположение пределов в nary‑операторах. Пределы могут быть либо центрированы над и под nary‑оператором, либо расположены сразу справа от оператора"
type: docs
url: /ru/net/aspose.cells.drawing.equations/naryequationnode/limitlocation/
---
## NaryEquationNode.LimitLocation property

Этот атрибут указывает расположение пределов в n-арных операторах. Пределы могут быть либо центрированы над и под n-арным оператором, либо расположены сразу справа от оператора.

```csharp
public EquationLimitLocationType LimitLocation { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyLimitLocationDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму для размещения уравнения
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // Получите доступ к уравнению и добавьте узел nary‑оператора
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // Привести к NaryEquationNode для доступа к LimitLocation
            var naryEquationNode = (NaryEquationNode)naryNode;

            try
            {
                // Отобразить текущий LimitLocation (значение по умолчанию)
                Console.WriteLine("Default LimitLocation: " + naryEquationNode.LimitLocation);

                // Установить LimitLocation в SubSup (пределы справа)
                naryEquationNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("After setting to SubSup: " + naryEquationNode.LimitLocation);

                // Вернуть обратно к UndOvr (центрированные пределы)
                naryEquationNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("After setting to UndOvr: " + naryEquationNode.LimitLocation);

                // Сохраните книгу
                workbook.Save("LimitLocationDemo.xlsx");
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

* enum [EquationLimitLocationType](../../equationlimitlocationtype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


