---
title: "CommentCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CommentCollection. تُضيف تعليقًا إلى المجموعة"
type: docs
url: /ar/net/aspose.cells/commentcollection/add/
---
## Add(int, int) {#add}

يضيف تعليقًا إلى المجموعة.

```csharp
public int Add(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس صف الخلية. |
| عمود | Int32 | فهرس عمود الخلية. |

### قيمة الإرجاع

[`Comment`](../../comment/) object index.

### أمثلة

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

### انظر أيضًا

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

يضيف تعليقًا إلى المجموعة.

```csharp
public int Add(string cellName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم الخلية. |

### قيمة الإرجاع

[`Comment`](../../comment/) object index.

### أمثلة

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

### انظر أيضًا

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


