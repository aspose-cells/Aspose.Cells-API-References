---
title: "Protection.AllowEditingObject"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Представляет, разрешено ли пользователю манипулировать графическими объектами на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/alloweditingobject/
---
## Protection.AllowEditingObject property

Представляет, разрешено ли пользователю манипулировать объектами рисования на защищённом листе.

```csharp
public bool AllowEditingObject { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите параметры защиты с включённым AllowEditingObject
            Protection protection = worksheet.Protection;
            protection.AllowEditingObject = true;
            protection.AllowEditingContent = false; // Contrast with AllowEditingObject
            worksheet.Protect(ProtectionType.All);

            // Проверьте флаги защиты
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowEditingObject: {protection.AllowEditingObject}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // Создайте текстовое поле (объект) для тестирования редактирования
            worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Сохраните книгу
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


