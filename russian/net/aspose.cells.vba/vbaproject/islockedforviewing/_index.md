---
title: "VbaProject.IslockedForViewing"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProject. Указывает, заблокирован ли этот проект VBA для просмотра"
type: docs
url: /ru/net/aspose.cells.vba/vbaproject/islockedforviewing/
---
## VbaProject.IslockedForViewing property

Указывает, заблокирован ли этот проект VBA для просмотра.

```csharp
[Obsolete("Use VbaProject.IsLockedForView property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IslockedForViewing { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство VbaProject.IsLockedForView. Это свойство будет удалено через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIslockedForViewingDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с проектом VBA
            Workbook wb = new Workbook();
            // Создайте новый лист, чтобы гарантировать создание VBA проекта
            wb.Worksheets.Add();
            
            // Продемонстрировать свойство IslockedForViewing
            Console.WriteLine("Initial state:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Защитить и заблокировать для просмотра
            wb.VbaProject.Protect(true, "password123");
            Console.WriteLine("After protecting and locking for viewing:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Защитить без блокировки для просмотра
            wb.VbaProject.Protect(false, "password456");
            Console.WriteLine("After protecting without locking for viewing:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Снять защиту
            wb.VbaProject.Protect(true, "");
            Console.WriteLine("After removing protection:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}");
        }
    }
}
```

### См. также

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


