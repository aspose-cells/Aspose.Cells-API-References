---
title: "LoadOptions.WarningCallback"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Получает или задает обратный вызов предупреждения"
type: docs
url: /ru/net/aspose.cells/loadoptions/warningcallback/
---
## LoadOptions.WarningCallback property

Получает или задаёт обратный вызов предупреждения.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.Description}");
        }
    }

    public class LoadOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Создайте пользовательский обратный вызов предупреждения
            IWarningCallback warningCallback = new CustomWarningCallback();

            // Инициализируйте параметры загрузки с обратным вызовом предупреждения
            LoadOptions options = new LoadOptions();
            options.WarningCallback = warningCallback;
            options.IgnoreUselessShapes = true;

            // Загрузить книгу с параметрами
            Workbook workbook = new Workbook("example.xlsx", options);

            // Продемонстрируйте использование обратного вызова предупреждения, получая доступ к ячейке
            Console.WriteLine($"Cell value: {workbook.Worksheets[0].Cells["A1"].StringValue}");

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* interface [IWarningCallback](../../iwarningcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


