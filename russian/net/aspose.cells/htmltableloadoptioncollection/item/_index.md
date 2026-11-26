---
title: "HtmlTableLoadOptionCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlTableLoadOptionCollection. Возвращает элемент HtmlTableLoadOption по указанному индексу"
type: docs
url: /ru/net/aspose.cells/htmltableloadoptioncollection/item/
---
## HtmlTableLoadOptionCollection indexer

Возвращает элемент [`HtmlTableLoadOption`](../../htmltableloadoption/) по указанному индексу.

```csharp
public HtmlTableLoadOption this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создайте HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Добавьте новый HtmlTableLoadOption по индексу таблицы
            int index1 = tableLoadOptions.Add(0);

            // Получить доступ к HtmlTableLoadOption с помощью свойства Item
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Настроить параметры загрузки таблицы
            option.TableToListObject = true;
            option.TargetSheetIndex = 1;

            // Загрузить HTML‑файл с настроенными параметрами
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


