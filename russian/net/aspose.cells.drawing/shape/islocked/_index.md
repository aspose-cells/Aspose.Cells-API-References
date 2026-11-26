---
title: "Shape.IsLocked"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. True означает, что объект нельзя изменить, когда лист защищён. Обратите внимание, что это значение имеет смысл только если лист или объекты на листе защищены"
type: docs
url: /ru/net/aspose.cells.drawing/shape/islocked/
---
## Shape.IsLocked property

True означает, что объект нельзя изменить, когда лист защищён. Обратите внимание, что это значение имеет смысл только если лист или объекты на листе защищены.

```csharp
public bool IsLocked { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsLockedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Защитить лист
            worksheet.Protect(ProtectionType.All);

            // Продемонстрируйте блокировку/разблокировку формы
            Console.WriteLine("Original IsLocked state: " + shape.IsLocked);

            // Разблокируйте форму
            shape.IsLocked = false;
            Console.WriteLine("After unlocking, IsLocked state: " + shape.IsLocked);

            // Заблокируйте форму
            shape.IsLocked = true;
            Console.WriteLine("After locking, IsLocked state: " + shape.IsLocked);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


