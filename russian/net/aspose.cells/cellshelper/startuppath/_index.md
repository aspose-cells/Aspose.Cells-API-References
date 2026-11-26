---
title: "CellsHelper.StartupPath"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsHelper. Получает или задает путь запуска, на который ссылаются некоторые внешние ссылки формул"
type: docs
url: /ru/net/aspose.cells/cellshelper/startuppath/
---
## CellsHelper.StartupPath property

Получает или задает путь запуска, на который ссылаются некоторые внешние формульные ссылки.

```csharp
public static string StartupPath { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyStartupPathDemo
    {
        public static void Run()
        {
            // Установить путь запуска
            CellsHelper.StartupPath = "C:\\Temp\\AsposeCellsStartup";
            
            // Отобразить путь запуска
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);

            // Продемонстрировать дополнительные свойства CellsHelper
            CellsHelper.SignificantDigits = 15;
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


