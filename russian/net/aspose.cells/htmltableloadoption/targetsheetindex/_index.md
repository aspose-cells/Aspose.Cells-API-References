---
title: "HtmlTableLoadOption.TargetSheetIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlTableLoadOption. Получить или задать целевой индекс листа, где будет расположена таблица"
type: docs
url: /ru/net/aspose.cells/htmltableloadoption/targetsheetindex/
---
## HtmlTableLoadOption.TargetSheetIndex property

Получите или задайте целевой индекс листа, где должна располагаться таблица.

```csharp
public int TargetSheetIndex { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTargetSheetIndexDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Настройте параметры загрузки таблицы с помощью TargetSheetIndex
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            tableLoadOption1.TargetSheetIndex = 0; // Load to first worksheet
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1; // Load to second worksheet
            
            // Добавить параметры загрузки таблицы
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);
            
            // Загрузить HTML‑файл с параметрами
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Проверьте, что таблицы загружены в правильные листы
            Console.WriteLine("Table1 loaded to sheet index: " + tableLoadOption1.TargetSheetIndex);
            Console.WriteLine("Table2 loaded to sheet index: " + tableLoadOption2.TargetSheetIndex);
        }
    }
}
```

### См. также

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


