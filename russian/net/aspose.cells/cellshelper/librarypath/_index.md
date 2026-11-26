---
title: "CellsHelper.LibraryPath"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsHelper. Получает или задает путь к библиотеке, на который ссылаются некоторые внешние формульные ссылки"
type: docs
url: /ru/net/aspose.cells/cellshelper/librarypath/
---
## CellsHelper.LibraryPath property

Получает или задает путь к библиотеке, на который ссылаются некоторые внешние формульные ссылки.

```csharp
public static string LibraryPath { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyLibraryPathDemo
    {
        public static void Run()
        {
            // Задать свойство LibraryPath
            CellsHelper.LibraryPath = "C:\\MyLibraries\\AsposeCells";

            // Продемонстрировать получение и использование LibraryPath
            Console.WriteLine("Current Library Path: " + CellsHelper.LibraryPath);

            // Пример использования пути в файловой операции
            string filePath = System.IO.Path.Combine(CellsHelper.LibraryPath, "test.xlsx");
            Console.WriteLine("Would load file from: " + filePath);
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


