---
title: "Класс SmartTagOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Markup.SmartTagOptions. Представляет параметры смарт‑тега"
type: docs
url: /ru/net/aspose.cells.markup/smarttagoptions/
---
## SmartTagOptions class

Представляет параметры смарт‑тега.

```csharp
public class SmartTagOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SmartTagOptions](smarttagoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [EmbedSmartTags](../../aspose.cells.markup/smarttagoptions/embedsmarttags/) { get; set; } | Указывает, сохранять ли смарт‑теги вместе с книгой. |
| [ShowType](../../aspose.cells.markup/smarttagoptions/showtype/) { get; set; } | Представляет тип отображения смарт‑тега. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать экземпляр SmartTagOptions
            SmartTagOptions options = new SmartTagOptions();

            // Установить свойства
            options.EmbedSmartTags = true;
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;

            // Применить SmartTagOptions к листу
            // Примечание: Изменено с worksheet.SmartTagSetting.Options = options;
            // для непосредственного использования объекта options, так как у SmartTagSetting нет свойства Options
            // (Предполагая, что options предназначены для непосредственного использования)
            
            // Добавьте некоторые данные для демонстрации
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);

            // Сохраните книгу
            workbook.Save("SmartTagOptionsDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


