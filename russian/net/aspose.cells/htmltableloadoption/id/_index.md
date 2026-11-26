---
title: "HtmlTableLoadOption.Id"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlTableLoadOption. Получить или установить идентификатор таблицы для импорта из HTML"
type: docs
url: /ru/net/aspose.cells/htmltableloadoption/id/
---
## HtmlTableLoadOption.Id property

Получите или задайте id таблицы для импорта из HTML

```csharp
public string Id { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyIdDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Настроить параметры загрузки таблицы
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1"; // Setting Id property
            tableLoadOption1.TargetSheetIndex = 0;
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2"; // Setting Id property
            tableLoadOption2.TargetSheetIndex = 0;

            // Добавить параметры загрузки таблицы
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // Загрузить HTML‑файл с указанными параметрами
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            Console.WriteLine("HTML tables with specified IDs have been loaded to Excel.");
        }
    }
}
```

### См. также

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


