---
title: "Класс SpreadsheetLocker"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.LowCode.SpreadsheetLocker. API низкого кода для блокировки файла электронной таблицы"
type: docs
url: /ru/net/aspose.cells.lowcode/spreadsheetlocker/
---
## SpreadsheetLocker class

API с низким кодом для блокировки файла электронной таблицы.

```csharp
public class SpreadsheetLocker
```

## Методы

| Имя | Описание |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) | Блокирует файл электронной таблицы с указанными настройками. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_1)(LowCodeLoadOptions, LowCodeSaveOptions, string, string) | Блокирует файл электронной таблицы с указанными настройками. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_3)(string, string, string, string) | Блокирует файл электронной таблицы с указанными настройками. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_2)(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) | Блокирует файл электронной таблицы с указанными настройками. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassSpreadsheetLockerDemo
    {
        public static void Run()
        {
            // Используйте SpreadsheetLocker для защиты рабочей книги
            SpreadsheetLocker.Process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


