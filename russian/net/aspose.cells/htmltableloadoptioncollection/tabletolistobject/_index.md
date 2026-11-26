---
title: "HtmlTableLoadOptionCollection.TableToListObject"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlTableLoadOptionCollection. Указывает, следует ли генерировать объекты списка из импортированных таблиц. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmltableloadoptioncollection/tabletolistobject/
---
## HtmlTableLoadOptionCollection.TableToListObject property

Указывает, следует ли генерировать объекты списка из импортированных таблиц. Значение по умолчанию — false.

```csharp
public bool TableToListObject { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();

            // Создайте HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Получите доступ к экземпляру HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Установите свойство TableToListObject, чтобы преобразовать HTML‑таблицы в ListObjects
            tableLoadOptions.TableToListObject = true;

            // Добавьте таблицу, которую нужно преобразовать в ListObject, по индексу
            tableLoadOptions.Add(0);

            // Загрузите HTML‑файл в рабочую книгу, используя параметры загрузки
            workbook = new Workbook("input.html", loadOptions);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


