---
title: "CommentCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CommentCollection. Добавляет комментарий в коллекцию"
type: docs
url: /ru/net/aspose.cells/commentcollection/add/
---
## Add(int, int) {#add}

Добавляет комментарий в коллекцию.

```csharp
public int Add(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки ячейки. |
| column | Int32 | Индекс столбца ячейки. |

### Возвращаемое значение

[`Comment`](../../comment/) object index.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            CommentCollection comments = worksheet.Comments;
            
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Font.Name = "Times New Roman";
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Добавляет комментарий в коллекцию.

```csharp
public int Add(string cellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки. |

### Возвращаемое значение

[`Comment`](../../comment/) object index.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CommentCollection comments = worksheet.Comments;
            
            int commentIndex1 = comments.Add("A1");
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Font.Name = "Arial";
            
            int commentIndex2 = comments.Add("B2");
            Comment comment2 = comments[commentIndex2];
            comment2.Note = "Second note.";
            comment2.Font.Name = "Times New Roman";
            
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### См. также

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


