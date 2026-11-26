---
title: "Workbook.GetStyleInPool"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Получает стиль из пула стилей. Все стили в рабочей книге собираются в пул. В ячейках хранится только простой индекс ссылки."
type: docs
url: /ru/net/aspose.cells/workbook/getstyleinpool/
---
## Workbook.GetStyleInPool method

Получает стиль из пула стилей. Все стили в рабочей книге будут собраны в пул. В ячейках присутствует только простой индекс ссылки.

```csharp
public Style GetStyleInPool(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс. |

### Возвращаемое значение

Стиль в пуле соответствует заданному индексу, может быть null.

### Примечания

Если изменён возвращённый стиль, стиль всех ячеек (которые ссылаются на этот стиль) будет изменён.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetStyleInPoolWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Получите доступ к первому листу и добавьте некоторые примерные данные
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123.45);
            ws.Cells["A3"].PutValue(DateTime.Now);
            
            // Применить некоторые стили
            Style style1 = wb.CreateStyle();
            style1.Custom = "$#,##0.00";
            ws.Cells["A2"].SetStyle(style1);
            
            Style style2 = wb.CreateStyle();
            style2.Custom = "yyyy-mm-dd";
            ws.Cells["A3"].SetStyle(style2);
            
            // Сохранить в поток памяти
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                
                // Перезагрузить рабочую книгу из потока
                ms.Position = 0;
                Workbook reloadWb = new Workbook(ms);
                
                // Получить и отобразить стили из пула стилей
                int count = reloadWb.CountOfStylesInPool;
                Console.WriteLine($"Styles in pool: {count}");
                
                for (int i = 0; i < count; i++)
                {
                    Style style = reloadWb.GetStyleInPool(i);
                    Console.WriteLine($"Style {i}: CustomFormat={style.Custom}");
                }
            }
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


