---
title: "Comment.Characters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Comment. Возвращает объект Characters, который представляет диапазон символов в тексте комментария"
type: docs
url: /ru/net/aspose.cells/comment/characters/
---
## Comment.Characters method

Возвращает объект Characters, который представляет диапазон символов внутри текста комментария.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | Int32 | Индекс начала символа. |
| длина | Int32 | Количество символов. |

### Возвращаемое значение

Объект Characters.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";
            
            // Получить настройку шрифта для первых 4 символов
            FontSetting fontSetting = comment1.Characters(0, 4);
            
            // Изменить настройки шрифта
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // Сохраните книгу
            workbook.Save("CommentFontSettingDemo.xlsx");
        }
    }
}
```

### См. также

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


