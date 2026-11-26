---
title: "CommentCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CommentCollection. Удаляет комментарий конкретной ячейки"
type: docs
url: /ru/net/aspose.cells/commentcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

Удаляет комментарий конкретной ячейки.

```csharp
public void RemoveAt(string cellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки, содержащей комментарий. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить комментарии в ячейки, используя имена ячеек
            int commentIndex1 = worksheet.Comments.Add("A1");
            worksheet.Comments[commentIndex1].Note = "Comment in A1";
            
            int commentIndex2 = worksheet.Comments.Add("B2");
            worksheet.Comments[commentIndex2].Note = "Comment in B2";
            
            int commentIndex3 = worksheet.Comments.Add("C3");
            worksheet.Comments[commentIndex3].Note = "Comment in C3";
            
            // Удалить комментарий в ячейке B2, используя RemoveAt со строковым параметром
            worksheet.Comments.RemoveAt("B2");
            
            // Сохраните книгу
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### См. также

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, int) {#removeat_1}

Удаляет комментарий конкретной ячейки.

```csharp
public void RemoveAt(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| column | Int32 | индекс столбца. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodRemoveAtWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить комментарии в ячейки, используя ссылки на ячейки
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";
            
            // Удалить комментарий в строке 1, столбце 1 (B2)
            worksheet.Comments.RemoveAt(1, 1);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


