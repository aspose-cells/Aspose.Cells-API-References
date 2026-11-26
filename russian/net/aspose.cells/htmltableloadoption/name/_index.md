---
title: "HtmlTableLoadOption.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlTableLoadOption. Получить или задать имя таблицы для импорта из html"
type: docs
url: /ru/net/aspose.cells/htmltableloadoption/name/
---
## HtmlTableLoadOption.Name property

Получить или задать имя таблицы для импорта из html

```csharp
[Obsolete("Please use HtmlTableLoadOption.Id instead")]
public string Name { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyNameDemo
    {
        public static void Run()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();

            // Создайте HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Получить доступ к HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Добавьте новый HtmlTableLoadOption по индексу таблицы
            int index = tableLoadOptions.Add(0);

            // Получить доступ к HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];

            // Установить свойство Name
            option.Name = "CustomerDataTable";

            // Загрузить HTML‑файл (замените реальным путём к файлу)
            workbook = new Workbook("input.html", loadOptions);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


