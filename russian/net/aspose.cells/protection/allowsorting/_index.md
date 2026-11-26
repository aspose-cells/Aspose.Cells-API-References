---
title: "Protection.AllowSorting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Представляет, разрешена ли опция сортировки на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/allowsorting/
---
## Protection.AllowSorting property

Представляет, разрешена ли опция сортировки на защищённом листе.

```csharp
public bool AllowSorting { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSortingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Включить защиту листа
            worksheet.Protect(ProtectionType.All);
            
            // Установите свойства защиты, включая AllowSorting
            Protection protection = worksheet.Protection;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowEditingContent = false;

            // Выведите параметры защиты
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowSorting: {protection.AllowSorting}");
            Console.WriteLine($"AllowFiltering: {protection.AllowFiltering}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // Продемонстрировать возможность сортировки
            if (protection.AllowSorting)
            {
                Console.WriteLine("\nSorting is allowed on this protected worksheet");
            }
            else
            {
                Console.WriteLine("\nSorting is not allowed on this protected worksheet");
            }
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


