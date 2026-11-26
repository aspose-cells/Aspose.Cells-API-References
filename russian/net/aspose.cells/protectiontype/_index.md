---
title: "Перечисление ProtectionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ProtectionType. Представляет тип защиты книги/листа."
type: docs
url: /ru/net/aspose.cells/protectiontype/
---
## ProtectionType enumeration

Представляет тип защиты книги/листа.

```csharp
public enum ProtectionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| All | `0` | Представляет защиту всех. |
| Contents | `1` | Представляет защиту содержимого, используется в защите листа. |
| Objects | `2` | Представляет защиту объектов, используется в защите листа. |
| Scenarios | `3` | Представляет защиту сценариев, используется в защите листа. |
| Structure | `4` | Представляет защиту структуры, используется в защите книги. |
| Windows | `5` | Представляет защиту окна, используется в защите книги. |
| None | `6` | Представляет отсутствие защиты. Только для свойства Reading. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectionTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Защитите лист всеми типами защиты
            worksheet.Protect(ProtectionType.All);
            
            // Продемонстрировать доступ к свойствам защиты
            Console.WriteLine("Worksheet protection settings:");
            Console.WriteLine("AllowDeletingColumn: " + worksheet.Protection.AllowDeletingColumn);
            Console.WriteLine("AllowDeletingRow: " + worksheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowFiltering: " + worksheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingCell: " + worksheet.Protection.AllowFormattingCell);
            Console.WriteLine("AllowFormattingColumn: " + worksheet.Protection.AllowFormattingColumn);
            Console.WriteLine("AllowFormattingRow: " + worksheet.Protection.AllowFormattingRow);
            Console.WriteLine("AllowInsertingColumn: " + worksheet.Protection.AllowInsertingColumn);
            Console.WriteLine("AllowInsertingHyperlink: " + worksheet.Protection.AllowInsertingHyperlink);
            Console.WriteLine("AllowInsertingRow: " + worksheet.Protection.AllowInsertingRow);
            Console.WriteLine("AllowSorting: " + worksheet.Protection.AllowSorting);
            Console.WriteLine("AllowUsingPivotTable: " + worksheet.Protection.AllowUsingPivotTable);
            
            // Снимите защиту с листа
            worksheet.Unprotect();
            
            // Защитить с использованием конкретных типов защиты
            worksheet.Protect(ProtectionType.Contents | ProtectionType.Objects);
            Console.WriteLine("\nWorksheet protected with Contents and Objects only");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


