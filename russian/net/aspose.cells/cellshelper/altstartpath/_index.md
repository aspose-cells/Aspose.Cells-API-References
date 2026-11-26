---
title: "CellsHelper.AltStartPath"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsHelper. Получает или задает альтернативный путь запуска, на который ссылаются некоторые внешние формульные ссылки"
type: docs
url: /ru/net/aspose.cells/cellshelper/altstartpath/
---
## CellsHelper.AltStartPath property

Получает или задает альтернативный путь запуска, на который ссылаются некоторые внешние формульные ссылки.

```csharp
public static string AltStartPath { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyAltStartPathDemo
    {
        public static void Run()
        {
            // Установите альтернативный путь запуска
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            
            // Также установите другие соответствующие свойства для демонстрации
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            
            // Отобразите пути, чтобы продемонстрировать использование свойства
            Console.WriteLine("Main Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            
            // Пример того, как могут использоваться эти пути
            Console.WriteLine("\nWhen resources aren't found in main path, system will check: " + CellsHelper.AltStartPath);
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


