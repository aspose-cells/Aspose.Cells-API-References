---
title: "VbaModule.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaModule. Получает тип модуля"
type: docs
url: /ru/net/aspose.cells.vba/vbamodule/type/
---
## VbaModule.Type property

Получает тип модуля.

```csharp
public VbaModuleType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyTypeDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу с примером файла, поддерживающего макросы
            Workbook wb = new Workbook("example.xlsm");
            
            // Получите доступ к VBA‑проекту и модулям
            VbaProject vbaProject = wb.VbaProject;
            VbaModuleCollection modules = vbaProject.Modules;
            
            // Отобразите типы модулей и их имена
            for (int i = 0; i < modules.Count; i++)
            {
                Console.WriteLine($"Module Name: {modules[i].Name}");
                Console.WriteLine($"Module Type: {modules[i].Type}");
                Console.WriteLine();
            }
            
            wb.Save("output.xlsm");
        }
    }
}
```

### См. также

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


