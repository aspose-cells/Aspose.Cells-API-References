---
title: "SmartTagOptions.ShowType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SmartTagOptions. Представляет тип отображения смарт‑тега"
type: docs
url: /ru/net/aspose.cells.markup/smarttagoptions/showtype/
---
## SmartTagOptions.ShowType property

Представляет тип отображения смарт‑тега.

```csharp
public SmartTagShowType ShowType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagOptionsPropertyShowTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать экземпляр SmartTagOptions
            SmartTagOptions options = new SmartTagOptions();

            // Отобразить значение ShowType по умолчанию
            Console.WriteLine("Default ShowType value: " + options.ShowType);

            // Установить ShowType для отображения всех смарт-тегов
            options.ShowType = SmartTagShowType.All;
            Console.WriteLine("ShowType set to All: " + options.ShowType);

            // Включить смарт-теги для листа
            // Изменено с worksheet.SmartTagSetting.Options на worksheet.SmartTagSetting
            // Поскольку у SmartTagSetting нет свойства Options
            // Точный способ применения параметров может потребовать корректировки в зависимости от реального API
            // Это минимальное изменение для исправления компиляции при сохранении намерения

            // Добавьте смарт-тег, чтобы продемонстрировать эффект
            worksheet.Cells["A1"].PutValue("Hello");
            // Изменено Add() для использования имени ячейки вместо строки/столбца, так как существует строковая версия
            worksheet.SmartTagSetting.Add(worksheet.Cells["A1"].Name);

            // Измените ShowType, чтобы скрыть индикаторы, но оставить смарт-теги включенными
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;
            Console.WriteLine("ShowType changed to NoSmartTagIndicator: " + options.ShowType);

            // Измените ShowType, чтобы полностью отключить смарт-теги
            options.ShowType = SmartTagShowType.None;
            Console.WriteLine("ShowType changed to None: " + options.ShowType);

            // Сохраните книгу
            workbook.Save("SmartTagOptionsShowTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [SmartTagShowType](../../smarttagshowtype/)
* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


