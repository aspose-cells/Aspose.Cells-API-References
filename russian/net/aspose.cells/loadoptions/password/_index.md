---
title: "LoadOptions.Password"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Получает и задает пароль рабочей книги"
type: docs
url: /ru/net/aspose.cells/loadoptions/password/
---
## LoadOptions.Password property

Получает и задает пароль рабочей книги.

```csharp
public string Password { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки и установить пароль
            LoadOptions options = new LoadOptions();
            options.Password = "test";

            // Загрузить книгу, защищённую паролем
            Workbook workbook = new Workbook("protected.xlsx", options);

            // Удалить защиту паролем после загрузки
            workbook.Settings.Password = null;

            // Сохранить незащищенный workbook
            workbook.Save("unprotected.xlsx");
        }
    }
}
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


