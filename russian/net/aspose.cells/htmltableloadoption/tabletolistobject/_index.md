---
title: "HtmlTableLoadOption.TableToListObject"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlTableLoadOption. Указывает, следует ли генерировать объекты списка из импортированной таблицы. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmltableloadoption/tabletolistobject/
---
## HtmlTableLoadOption.TableToListObject property

Указывает, следует ли генерировать объекты списка из импортированной таблицы. Значение по умолчанию — false.

```csharp
public bool TableToListObject { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();

            // Создайте параметры загрузки HTML с включённым TableToListObject
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Загрузить HTML с указанными параметрами
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


