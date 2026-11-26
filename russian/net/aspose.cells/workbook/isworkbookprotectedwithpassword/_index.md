---
title: "Workbook.IsWorkbookProtectedWithPassword"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Указывает, защищены ли структура или окно паролем"
type: docs
url: /ru/net/aspose.cells/workbook/isworkbookprotectedwithpassword/
---
## Workbook.IsWorkbookProtectedWithPassword property

Указывает, защищены ли структура или окно паролем.

```csharp
public bool IsWorkbookProtectedWithPassword { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsWorkbookProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // Создать новый экземпляр Workbook
            Workbook workbook = new Workbook();

            // Проверьте, защищена ли рабочая книга паролем (для новой книги должно быть false)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Защитить книгу паролем
            workbook.Protect(ProtectionType.All, "password123");

            // Теперь проверьте снова (должно быть true)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Снимите защиту с рабочей книги
            workbook.Unprotect("password123");

            // Последняя проверка (должно быть false снова)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Освободить ресурсы книги
            workbook.Dispose();
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


