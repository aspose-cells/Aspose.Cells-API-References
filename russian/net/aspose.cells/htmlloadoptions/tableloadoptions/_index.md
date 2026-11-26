---
title: "HtmlLoadOptions.TableLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlLoadOptions. Получить экземпляр HtmlTableLoadOptionCollection"
type: docs
url: /ru/net/aspose.cells/htmlloadoptions/tableloadoptions/
---
## HtmlLoadOptions.TableLoadOptions property

Получить экземпляр HtmlTableLoadOptionCollection

```csharp
public HtmlTableLoadOptionCollection TableLoadOptions { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyTableLoadOptionsDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            
            // Добавить параметры загрузки таблицы по индексу
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            
            // Добавить параметры загрузки таблицы по идентификатору
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table2";
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Загрузите HTML‑файл с использованием параметров
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Сохранить вывод
            workbook.Save("output.xlsx");
            
            // Очистить и добавить новые параметры загрузки таблицы
            loadOptions.TableLoadOptions.Clear();
            
            // Добавить параметры загрузки таблицы с сопоставлением индекса листа
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 -> Sheet 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 -> Sheet 0
            
            // Добавить параметры загрузки таблицы с идентификатором и сопоставлением листа
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "mainTable";
            tableLoadOption.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            // Загрузить и снова сохранить с новыми параметрами
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output_mapped.xlsx");
        }
    }
}
```

### См. также

* class [HtmlTableLoadOptionCollection](../../htmltableloadoptioncollection/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


