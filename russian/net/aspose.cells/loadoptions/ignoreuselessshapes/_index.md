---
title: "LoadOptions.IgnoreUselessShapes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Указывает, следует ли игнорировать бесполезные фигуры"
type: docs
url: /ru/net/aspose.cells/loadoptions/ignoreuselessshapes/
---
## LoadOptions.IgnoreUselessShapes property

Указывает, следует ли игнорировать бесполезные фигуры.

```csharp
public bool IgnoreUselessShapes { get; set; }
```

### Примечания

Работает только с файлами xlsx, xlsb и xlsm. Существует множество перекрывающихся одинаковых фигур, которые в некоторых файлах бесполезны; их можно игнорировать при загрузке файлов.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreUselessShapesDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки и установить IgnoreUselessShapes в true
            LoadOptions options = new LoadOptions();
            options.IgnoreUselessShapes = true;

            // Загрузите книгу с параметрами
            Workbook workbook = new Workbook("example.xlsx", options);

            // Вывести количество фигур в первом листе
            Console.WriteLine("Shapes count: " + workbook.Worksheets[0].Shapes.Count);
        }
    }
}
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


