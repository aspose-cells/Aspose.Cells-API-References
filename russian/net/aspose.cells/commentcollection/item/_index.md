---
title: "CommentCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CommentCollection. Возвращает элемент Comment по указанному индексу"
type: docs
url: /ru/net/aspose.cells/commentcollection/item/
---
## CommentCollection indexer (1 of 3)

Возвращает элемент [`Comment`](../../comment/) по указанному индексу.

```csharp
public Comment this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте комментарии в ячейки
            int commentIndex1 = worksheet.Comments.Add("A1");
            int commentIndex2 = worksheet.Comments.Add("B2");
            
            // Доступ к комментариям с помощью свойства Item
            Comment comment1 = worksheet.Comments[commentIndex1];
            Comment comment2 = worksheet.Comments[commentIndex2];
            
            // Установить заметки к комментариям
            comment1.Note = "First comment";
            comment2.Note = "Second comment";
            
            // Изменить первый комментарий с помощью свойства Item
            worksheet.Comments[0].Note = "Updated first comment";
            
            // Получать и изменять комментарий напрямую из коллекции
            Comment comment3 = worksheet.Comments[1];
            comment3.Note = "Updated second comment";
            
            // Сохраните книгу
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (2 of 3)

Возвращает элемент [`Comment`](../../comment/) по указанной ячейке.

```csharp
public Comment this[string cellName] { get; }
```

| Параметр | Описание |
| --- | --- |
| cellName | Имя ячейки. |

### Возвращаемое значение

Элемент в указанной ячейке.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарии в ячейки, используя ссылки на ячейки
            int comment1Index = worksheet.Comments.Add(0, 0); // A1
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add(1, 1); // B2
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add(2, 2); // C3
            worksheet.Comments[comment3Index].Note = "Third comment";

            // Получить доступ к комментариям с помощью свойства Item с ссылками на ячейки
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments["A1"];
            Comment comment2 = comments["B2"];
            Comment comment3 = comments["C3"];

            // Изменить заметки комментариев
            comment1.Note = "Updated first note";
            comment2.Note = "Updated second note";
            comment3.Note = "Updated third note";

            // Сохраните книгу
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (3 of 3)

Получает элемент [`Comment`](../../comment/) по указанному индексу строки и индексу столбца.

```csharp
public Comment this[int row, int column] { get; }
```

| Параметр | Описание |
| --- | --- |
| строка | Индекс строки. |
| column | Индекс столбца. |

### Возвращаемое значение

Элемент в указанной ячейке.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарии в ячейки, используя ссылки на ячейки
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";

            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";

            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";

            // Получить доступ к комментариям с помощью свойства Item с индексами строки/столбца
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments[0, 0];
            comment1.Note = "Updated first comment";

            Comment comment2 = comments[1, 1];
            comment2.Note = "Updated second comment";

            // Сохраните книгу
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


