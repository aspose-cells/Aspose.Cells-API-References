---
title: "Workbook.Unprotect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Снимает защиту с workbook"
type: docs
url: /ru/net/aspose.cells/workbook/unprotect/
---
## Workbook.Unprotect method

Снимает защиту с книги.

```csharp
public void Unprotect(string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| пароль | String | Пароль для снятия защиты с workbook. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // Создать workbook с защитой
            Workbook workbook = new Workbook();
            workbook.Protect(ProtectionType.All, "book");

            // Снимите защиту с workbook с правильным паролем
            workbook.Unprotect("book");

            // Сохранить незащищенный workbook
            workbook.Save("unprotected_workbook.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


