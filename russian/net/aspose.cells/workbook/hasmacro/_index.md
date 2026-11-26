---
title: "Workbook.HasMacro"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Указывает, содержит ли эта электронная таблица макрос/VBA"
type: docs
url: /ru/net/aspose.cells/workbook/hasmacro/
---
## Workbook.HasMacro property

Указывает, содержит ли эта электронная таблица макросы/VBA.

```csharp
public bool HasMacro { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasMacroDemo
    {
        public static void Run()
        {
            // Создать рабочую книгу с макросом, загрузив файл шаблона
            Workbook workbookWithMacro = new Workbook("sample_with_macro.xlsm");
            Console.WriteLine("Workbook with macro - HasMacro: " + workbookWithMacro.HasMacro);

            // Создать рабочую книгу без макроса
            Workbook workbookWithoutMacro = new Workbook();
            Console.WriteLine("Workbook without macro - HasMacro: " + workbookWithoutMacro.HasMacro);
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


