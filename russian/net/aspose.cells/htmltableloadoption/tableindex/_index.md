---
title: "HtmlTableLoadOption.TableIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlTableLoadOption. Получить или задать индекс таблицы для импорта из html"
type: docs
url: /ru/net/aspose.cells/htmltableloadoption/tableindex/
---
## HtmlTableLoadOption.TableIndex property

Получите или задайте индекс таблицы для импорта из HTML.

```csharp
public int TableIndex { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableIndexDemo
    {
        public static void Run()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();

            // Создать параметры загрузки HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Настройте параметр загрузки таблицы с TableIndex = 0 (первая таблица)
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };

            // Добавьте параметр загрузки таблицы
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Загрузить HTML‑файл (замените реальным путём)
            workbook = new Workbook("input.html", loadOptions);

            // Сохранить как файл Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


