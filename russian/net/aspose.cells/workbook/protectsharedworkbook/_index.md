---
title: "Workbook.ProtectSharedWorkbook"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Защищает общую книгу"
type: docs
url: /ru/net/aspose.cells/workbook/protectsharedworkbook/
---
## Workbook.ProtectSharedWorkbook method

Защищает общую книгу.

```csharp
public void ProtectSharedWorkbook(string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| пароль | String | Пароль для защиты книги. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodProtectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Защитите общую книгу паролем
            wb.ProtectSharedWorkbook("abcd");
            
            // Сохранить защищённую книгу
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // Загрузить защищённую книгу
            Workbook wbProtected = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // Проверить статус защиты
            Console.WriteLine("Workbook is protected: " + wbProtected.Settings.IsProtected);
            
            // Снимите защиту с рабочей книги
            wbProtected.UnprotectSharedWorkbook("abcd");
            
            // Сохранить незащищенный workbook
            wbProtected.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


