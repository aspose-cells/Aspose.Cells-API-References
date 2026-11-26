---
title: "Класс LowCodeMergeOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.LowCode.LowCodeMergeOptions класс. Параметры для объединения нескольких файлов шаблонов в один"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodemergeoptions/
---
## LowCodeMergeOptions class

Параметры объединения нескольких файлов шаблонов в один.

```csharp
public class LowCodeMergeOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LowCodeMergeOptions](lowcodemergeoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [LoadOptionsProvider](../../aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/) { get; set; } | Провайдер параметров сохранения для сохранения разделённых частей. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodemergeoptions/saveoptions/) { get; set; } | Параметры сохранения для сохранения разделённых частей. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeMergeOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создайте и настройте LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            
            // Установите параметры сохранения для выходного формата
            mergeOptions.SaveOptions = new LowCodeSaveOptions();
            
            // Назначьте пользовательского поставщика параметров загрузки
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();
            
            // Пример интеграции (гипотетическое использование с функцией объединения)
            // Обычно это вызывается с реальными путями к файлам
            // Workbook.Merge(new string[] { "template1.xlsx", "template2.xlsx" }, mergeOptions);
            
            // Сохраните книгу (для демонстрационных целей)
            workbook.Save("LowCodeMergeOptionsDemo.xlsx");
        }
    }

    // Пользовательский поставщик, реализующий абстрактный класс
    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {
        public override bool MoveNext()
        {
            // Минимальная реализация для удовлетворения требований абстракции
            return false;
        }

        public override LowCodeLoadOptions Current
        {
            get { throw new InvalidOperationException(); }
        }

        public LoadOptions GetLoadOptions(string fileName)
        {
            if (fileName.EndsWith(".xlsx", StringComparison.OrdinalIgnoreCase))
            {
                return new LoadOptions(LoadFormat.Xlsx);
            }
            return new LoadOptions();
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


