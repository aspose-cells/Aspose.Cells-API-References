---
title: "Класс AbstractLowCodeLoadOptionsProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.LowCode.AbstractLowCodeLoadOptionsProvider класс. Реализация для предоставления множества параметров загрузки для процессов, использующих несколько входных данных, таких как файлы шаблонов"
type: docs
url: /ru/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/
---
## AbstractLowCodeLoadOptionsProvider class

Реализация, предоставляющая несколько вариантов загрузки для процессов, использующих несколько входных данных (например, файлов шаблонов).

```csharp
public abstract class AbstractLowCodeLoadOptionsProvider
```

## Свойства

| Имя | Описание |
| --- | --- |
| abstract [Current](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/) { get; } | Получает параметры загрузки, из которых загружать данные текущей обрабатываемой части. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/)(LowCodeLoadOptions) | Освобождает ресурсы после обработки текущей части входных данных. |
| abstract [MoveNext](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/movenext/)() | Проверяет, есть ли ещё входные данные. |

### Примечания

Например, функция [`SpreadsheetMerger`](../spreadsheetmerger/) требует нескольких файлов шаблонов для объединения.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // Создайте пользовательскую реализацию AbstractLowCodeLoadOptionsProvider
            var provider = new CustomLoadOptionsProvider();

            // Обрабатывайте несколько входов с помощью провайдера
            while (provider.MoveNext())
            {
                // Получить текущие параметры загрузки
                LowCodeLoadOptions currentOptions = provider.Current;
                Console.WriteLine($"Processing with load options: {currentOptions}");

                // Создать рабочую книгу с текущими параметрами
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                Worksheet worksheet = workbook.Worksheets[0];

                // Продемонстрировать использование с рабочей книгой
                worksheet.Cells["A1"].PutValue("Processed with custom provider");
                
                // Завершить обработку этой части
                provider.Finish(currentOptions);
            }
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int currentIndex = 0;
            private readonly LowCodeLoadOptions[] optionsList = new LowCodeLoadOptions[]
            {
                new LowCodeLoadOptions(),
                new LowCodeLoadOptions { InputFile = "protected.xlsx" }, // Password would be handled separately
                new LowCodeLoadOptions() // MemorySetting would be handled separately
            };

            public override LowCodeLoadOptions Current => optionsList[currentIndex];

            public override bool MoveNext()
            {
                if (currentIndex < optionsList.Length - 1)
                {
                    currentIndex++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // Логика очистки или завершения для каждой части
                Console.WriteLine($"Finished processing part {currentIndex}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


