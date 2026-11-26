---
title: "PageSetup.PrintTitleColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет столбцы, содержащие ячейки, повторяющиеся слева на каждой странице"
type: docs
url: /ru/net/aspose.cells/pagesetup/printtitlecolumns/
---
## PageSetup.PrintTitleColumns property

Отображает столбцы, содержащие ячейки, которые повторяются слева от каждой страницы.

```csharp
public string PrintTitleColumns { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleColumnsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Доступ к настройкам страницы
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Установить повторение столбца A в заголовках печати на каждой печатной странице
            pageSetup.PrintTitleColumns = "$A:$A";
            
            // Добавьте некоторые данные в столбец A, чтобы продемонстрировать эффект
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[$"A{i + 1}"].PutValue($"Title Column - Row {i + 1}");
            }
            
            // Сохраните книгу
            workbook.Save("PrintTitleColumnsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


