---
title: "Workbook.StartAccessCache"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Запускает сеанс, использующий кэши для доступа к данным"
type: docs
url: /ru/net/aspose.cells/workbook/startaccesscache/
---
## Workbook.StartAccessCache method

Запускает сеанс, использующий кэш для доступа к данным.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| opts | AccessCacheOptions | параметры доступа к данным |

### Примечания

Если кэш указанного доступа к данным требует, чтобы некоторые модели данных в листе были «только для чтения», то соответствующие модели данных во всех листах этой книги будут считаться «только для чтения», и пользователь не должен изменять их. После завершения доступа к данным следует вызвать [`CloseAccessCache`](../closeaccesscache/) с теми же параметрами, чтобы очистить все кэши и восстановить обычный режим доступа.

### Примеры

```csharp
using System;
using System.Drawing;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавить условное форматирование
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            int index = cfc.Add();
            cfc[index].Add(CellArea.CreateCellArea(0, 0, 5, 0),
                FormatConditionType.DuplicateValues, OperatorType.None, null, null);
            
            // Установить стиль для условного форматирования
            Style style = cfc[0][0].Style;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            
            // Добавить несколько встроенных изображений
            Cells cells = sheet.Cells;
            byte[] img1 = File.ReadAllBytes("1.png");
            byte[] img2 = File.ReadAllBytes("2.png");
            cells[0, 0].EmbeddedImage = img1;
            cells[2, 0].EmbeddedImage = img2;
            cells[4, 0].EmbeddedImage = img1;

            // Запустить кэш доступа для повышения производительности
            wb.StartAccessCache(AccessCacheOptions.All);
            
            // Получить доступ к стилям ячеек (будет быстрее благодаря кэшированию)
            Console.WriteLine("A1 Pattern: " + cells[0, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A3 Pattern: " + cells[2, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A5 Pattern: " + cells[4, 0].GetDisplayStyle().Pattern);
            
            // Закрыть кэш после завершения
            wb.CloseAccessCache(AccessCacheOptions.All);
        }
    }
}
```

### См. также

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


