---
title: "Workbook.RemoveUnusedStyles"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Удалить все неиспользуемые стили"
type: docs
url: /ru/net/aspose.cells/workbook/removeunusedstyles/
---
## Workbook.RemoveUnusedStyles method

Удалить все неиспользуемые стили.

```csharp
public void RemoveUnusedStyles()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveUnusedStylesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавьте некоторые примерные данные со стилями
            for (int i = 0; i < 10; i++)
            {
                Cell cell = sheet.Cells[i, 0];
                cell.PutValue("Item " + (i + 1));
                
                // Примените разные стили к ячейкам
                Style style = wb.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 10 + i;
                style.Font.IsBold = i % 2 == 0;
                cell.SetStyle(style);
            }
            
            // Удалите некоторые ячейки, чтобы оставить неиспользуемые стили
            sheet.Cells.DeleteRows(5, 5);
            
            // Сохраните перед удалением неиспользуемых стилей
            wb.Save("BeforeRemoveUnusedStyles.xlsx");
            
            // Удалить неиспользуемые стили
            wb.RemoveUnusedStyles();
            
            // Сохранить после удаления неиспользуемых стилей
            wb.Save("AfterRemoveUnusedStyles.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


