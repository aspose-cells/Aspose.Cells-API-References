---
title: "LowCodeSplitOptions.LoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSplitOptions. Параметры загрузки для загрузки таблицы, которая будет разделена"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesplitoptions/loadoptions/
---
## LowCodeSplitOptions.LoadOptions property

Параметры загрузки для загрузки электронной таблицы, которая будет разделена.

```csharp
public LowCodeLoadOptions LoadOptions { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertyLoadOptionsDemo
    {
        public static void Run()
        {
            // Создайте экземпляр параметров разделения
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // Инициализировать параметры загрузки
            splitOptions.LoadOptions = new LowCodeLoadOptions();

            // Создайте новые параметры загрузки с различными настройками (используя доступные свойства)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // Продемонстрируйте окончательную конфигурацию
            Console.WriteLine("LoadOptions configured with InputFile: " + splitOptions.LoadOptions.InputFile);
        }
    }
}
```

### См. также

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


