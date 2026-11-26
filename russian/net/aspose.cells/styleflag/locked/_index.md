---
title: "StyleFlag.Locked"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Параметр Locked будет применён"
type: docs
url: /ru/net/aspose.cells/styleflag/locked/
---
## StyleFlag.Locked property

Настройка блокировки будет применена.

```csharp
public bool Locked { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLockedDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создайте стиль и установите его свойство locked
            Style style = workbook.CreateStyle();
            style.IsLocked = true;

            // Создайте флаг стиля и включите флаг locked
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Locked = true;

            // Применить стиль к ячейке A1
            Cell cell = cells["A1"];
            cell.SetStyle(style, styleFlag);

            // Проверьте статус locked
            Console.WriteLine("Cell A1 is locked: " + cell.GetStyle().IsLocked);

            // Защитите лист, чтобы увидеть эффект блокировки
            worksheet.Protect(ProtectionType.All);

            // Попробуйте изменить заблокированную ячейку (будет выброшено исключение, когда лист защищён)
            try
            {
                cell.PutValue("Test");
                Console.WriteLine("Cell modified successfully (worksheet not properly protected)");
            }
            catch
            {
                Console.WriteLine("Could not modify locked cell (worksheet protected)");
            }
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


