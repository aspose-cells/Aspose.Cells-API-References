---
title: "Workbook.RemoveMacro"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Удаляет VBA/макрос из этой электронной таблицы"
type: docs
url: /ru/net/aspose.cells/workbook/removemacro/
---
## Workbook.RemoveMacro method

Удаляет VBA/макрос из этой таблицы.

```csharp
public void RemoveMacro()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveMacroDemo
    {
        public static void Run()
        {
            // Создать книгу из существующего файла с поддержкой макросов
            Workbook workbook = new Workbook("example.xlsm");

            // Удалить макросы из книги
            workbook.RemoveMacro();
            
            // Сохранить как книгу без макросов
            string noMacroPath = "NoMacro.xlsx";
            workbook.Save(noMacroPath, SaveFormat.Xlsx);

            Console.WriteLine("Macros removed successfully. File created: " + noMacroPath);
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


