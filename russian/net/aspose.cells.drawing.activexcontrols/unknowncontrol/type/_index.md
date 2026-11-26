---
title: "UnknownControl.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство UnknownControl. Получает тип ActiveX‑контролла"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/unknowncontrol/type/
---
## UnknownControl.Type property

Получает тип ActiveX‑элемента управления.

```csharp
public override ControlType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class UnknownControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Загрузить существующий workbook, содержащий неизвестный контрол
            Workbook workbook = new Workbook("input_with_unknown_control.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];

            // Найти и обработать экземпляры UnknownControl
            foreach (Shape shape in worksheet.Shapes)
            {
                if (shape.ActiveXControl is UnknownControl control)
                {
                    // Продемонстрировать чтение свойства Type
                    Console.WriteLine($"Found control with Type: {control.Type}");
                    
                    // Пример использования, основанный на типе контролла
                    if (control.Type == ControlType.ListBox)
                    {
                        Console.WriteLine("Processing legacy ListBox control");
                    }
                    else if (control.Type == ControlType.Unknown)
                    {
                        Console.WriteLine("Handling completely unknown control type");
                    }
                }
            }

            // Сохранить обработанную книгу
            workbook.Save("ControlTypeAnalysis.xlsx");
        }
    }
}
```

### См. также

* enum [ControlType](../../controltype/)
* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


