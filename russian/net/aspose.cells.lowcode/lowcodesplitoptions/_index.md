---
title: "Класс LowCodeSplitOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.LowCode.LowCodeSplitOptions. Параметры для разделения электронных таблиц"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesplitoptions/
---
## LowCodeSplitOptions class

Параметры разделения электронной таблицы.

```csharp
public class LowCodeSplitOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LowCodeSplitOptions](lowcodesplitoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [LoadOptions](../../aspose.cells.lowcode/lowcodesplitoptions/loadoptions/) { get; set; } | Параметры загрузки для загрузки электронной таблицы, которая будет разделена. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptions/) { get; set; } | Параметры сохранения для сохранения разделённых частей. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/) { get; set; } | Провайдер параметров сохранения для сохранения разделённых частей. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeSplitOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполнить лист образцовыми данными
            worksheet.Cells["A1"].PutValue("Sample Data for Splitting");
            
            // Создайте экземпляр LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // Настройте LoadOptions (пример: обработка защищённого паролем источника)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // Настройте SaveOptions (пример: установить формат вывода по умолчанию)
            splitOptions.SaveOptions = new LowCodeSaveOptions();
            
            // Реализуйте пользовательский провайдер SaveOptions для динамических настроек вывода
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // Пример интеграции: разделите книгу на части, используя настроенные параметры
            // (Предположим наличие метода вроде LowCodeEngine.Split(workbook, splitOptions, "outputDir"))
            // LowCodeEngine.Split(workbook, splitOptions, "OutputDirectory");
            
            // Сохраните оригинальную книгу для демонстрации
            workbook.Save("LowCodeSplitOptionsDemo.xlsx");
        }

        // Реализация пользовательского SaveOptionsProvider
        private class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // Пример логики: чередовать настройки в зависимости от индекса разделения
                return new LowCodeSaveOptions();
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


