---
title: "LowCodeMergeOptions.LoadOptionsProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeMergeOptions. Провайдер параметров сохранения для сохранения разделённых частей"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/
---
## LowCodeMergeOptions.LoadOptionsProvider property

Провайдер параметров сохранения для сохранения разделённых частей.

```csharp
public AbstractLowCodeLoadOptionsProvider LoadOptionsProvider { get; set; }
```

### Примечания

Если это свойство указано, [`LoadOptions`](../../../aspose.cells/loadoptions/) не будет иметь эффекта, потому что вывод каждой разделённой части будет определён провайдером.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeMergeOptionsPropertyLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать экземпляр LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();

            // Отобразить текущее значение LoadOptionsProvider (по умолчанию должно быть null)
            Console.WriteLine("Current LoadOptionsProvider value: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // Создать пользовательскую реализацию LoadOptionsProvider
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();

            // Продемонстрировать установку свойства
            Console.WriteLine("After setting LoadOptionsProvider: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // Использовать параметры слияния с провайдером
            // Обычно это используется с методами, обрабатывающими несколько файлов
            // Для демонстрации мы просто проверим, может ли провайдер перейти к следующему
            bool hasNext = mergeOptions.LoadOptionsProvider.MoveNext();
            Console.WriteLine("LoadOptionsProvider MoveNext result: " + hasNext);

            // Сохраните книгу
            workbook.Save("PropertyLoadOptionsProviderDemo.xlsx");
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int counter = 0;
            private readonly LowCodeLoadOptions options = new LowCodeLoadOptions();

            public override LowCodeLoadOptions Current => options;

            public override bool MoveNext()
            {
                // Смоделировать наличие 3 файлов для обработки
                if (counter < 3)
                {
                    counter++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // Здесь будет логика очистки или завершения
            }
        }
    }
}
```

### См. также

* class [AbstractLowCodeLoadOptionsProvider](../../abstractlowcodeloadoptionsprovider/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


