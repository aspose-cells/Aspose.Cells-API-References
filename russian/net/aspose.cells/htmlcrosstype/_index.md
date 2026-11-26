---
title: "Перечисление HtmlCrossType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.HtmlCrossType. Представляет пять типов html cross string"
type: docs
url: /ru/net/aspose.cells/htmlcrosstype/
---
## HtmlCrossType enumeration

Представляет пять типов HTML‑перекрёстных строк.

```csharp
public enum HtmlCrossType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Default | `0` | Отображать как в MS Excel, зависит от следующей ячейки. Если следующая ячейка null, строка будет пересекаться, иначе будет обрезана |
| MSExport | `1` | Отображать строку как в MS Excel при экспорте html. |
| Cross | `2` | Отображать HTML cross string, эта производительность при создании больших html‑файлов будет более чем в десять раз быстрее, чем установка значения Default или FitToCell. |
| CrossHideRight | `3` | Отображать HTML cross string и скрывать правую строку, когда тексты перекрываются. |
| FitToCell | `4` | Отображать строку только в пределах ширины ячейки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHtmlCrossTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);
            
            // Создать параметры сохранения HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Установить тип пересечения в MSExport
            options.HtmlCrossStringType = HtmlCrossType.MSExport;
            
            // Сохранить книгу с параметрами HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with HtmlCrossType.MSExport");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


