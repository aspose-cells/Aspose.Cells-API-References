---
title: "Workbook.UnprotectSharedWorkbook"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Снимает защиту с общей книги"
type: docs
url: /ru/net/aspose.cells/workbook/unprotectsharedworkbook/
---
## Workbook.UnprotectSharedWorkbook method

Снимает защиту с общей книги.

```csharp
public void UnprotectSharedWorkbook(string password)
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
    public class WorkbookMethodUnprotectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Защитите общую книгу паролем
            wb.ProtectSharedWorkbook("abcd");
            
            // Сохранить защищённую книгу
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // Повторно открыть рабочую книгу
            wb = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // Снимите защиту с общей книги с помощью пароля
            wb.UnprotectSharedWorkbook("abcd");
            
            // Сохранить незащищенный workbook
            wb.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


