---
title: "Style.IsModified"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Style. Проверяет, были ли изменены указанные свойства стиля. Используется для стилей ConditionalFormattings, чтобы проверить, следует ли использовать указанные свойства этого стиля при применении ConditionalFormattings к ячейке."
type: docs
url: /ru/net/aspose.cells/style/ismodified/
---
## Style.IsModified method

Проверяет, были ли изменены указанные свойства стиля. Используется для стиля ConditionalFormattings, чтобы проверить, следует ли использовать указанные свойства этого стиля при применении ConditionalFormattings к ячейке.

```csharp
public bool IsModified(StyleModifyFlag modifyFlag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| modifyFlag | StyleModifyFlag | Флаги изменённого стиля |

### Возвращаемое значение

true, если указанные свойства были изменены

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodIsModifiedWithStyleModifyFlagDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить стиль ячейки A1
            Style style = worksheet.Cells["A1"].GetStyle();
            
            // Изменить узор (фон) стиля
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            
            // Проверьте, был ли изменён узор
            bool isPatternModified = style.IsModified(StyleModifyFlag.Pattern);
            
            // Вывести результат.
            Console.WriteLine("Is pattern modified: " + isPatternModified);
        }
    }
}
```

### См. также

* enum [StyleModifyFlag](../../stylemodifyflag/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


