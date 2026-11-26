---
title: "Shape.RemoveActiveXControl"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Удалить activeX control"
type: docs
url: /ru/net/aspose.cells.drawing/shape/removeactivexcontrol/
---
## Shape.RemoveActiveXControl method

Удалить элемент управления ActiveX.

```csharp
public void RemoveActiveXControl()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodRemoveActiveXControlDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте shape, который будет содержать ActiveX control
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.CommandButton, 
                1, 1, 1, 1, 100, 50);
            
            // Удалите ActiveX control, если он существует
            if (shape.ActiveXControl != null)
            {
                shape.RemoveActiveXControl();
                Console.WriteLine("ActiveX control removed successfully.");
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


