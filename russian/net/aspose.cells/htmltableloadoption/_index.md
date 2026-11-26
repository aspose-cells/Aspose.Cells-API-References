---
title: "Класс HtmlTableLoadOption"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.HtmlTableLoadOption. Представляет параметр при импорте таблицы из HTML"
type: docs
url: /ru/net/aspose.cells/htmltableloadoption/
---
## HtmlTableLoadOption class

Представляет параметр при импорте таблицы из HTML.

```csharp
public class HtmlTableLoadOption
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [HtmlTableLoadOption](htmltableloadoption/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Id](../../aspose.cells/htmltableloadoption/id/) { get; set; } | Получите или задайте id таблицы для импорта из HTML |
| [Name](../../aspose.cells/htmltableloadoption/name/) { get; set; } | (**Устарело.**) Получите или задайте имя таблицы для импорта из HTML |
| [OriginalSheetIndex](../../aspose.cells/htmltableloadoption/originalsheetindex/) { get; set; } | Получите или задайте оригинальный индекс листа в HTML. |
| [TableIndex](../../aspose.cells/htmltableloadoption/tableindex/) { get; set; } | Получите или задайте индекс таблицы для импорта из HTML. |
| [TableToListObject](../../aspose.cells/htmltableloadoption/tabletolistobject/) { get; set; } | Указывает, следует ли генерировать объекты списка из импортированной таблицы. Значение по умолчанию — false. |
| [TargetSheetIndex](../../aspose.cells/htmltableloadoption/targetsheetindex/) { get; set; } | Получите или задайте целевой индекс листа, где должна располагаться таблица. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionDemo
    {
        public static void HtmlTableLoadOptionExample()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();

            // Создать экземпляр HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Создайте экземпляр HtmlTableLoadOption
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                Id = "table1",
                Name = "SampleTable",
                OriginalSheetIndex = 0,
                TargetSheetIndex = 0,
                TableToListObject = true
            };

            // Добавьте HtmlTableLoadOption в HtmlLoadOptions
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Загрузите HTML‑файл в книгу с указанными параметрами загрузки
            workbook = new Workbook("HtmlTableLoadOptionExample_original.html", loadOptions);

            // Сохраните Workbook в файл Excel
            workbook.Save("HtmlTableLoadOptionExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


