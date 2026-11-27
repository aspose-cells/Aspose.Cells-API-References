---
title: "CommentCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CommentCollection-metod. Lägger till en kommentar i samlingen"
type: docs
url: /sv/net/aspose.cells/commentcollection/add/
---
## Add(int, int) {#add}

Lägger till en kommentar i samlingen.

```csharp
public int Add(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Cellradindex. |
| column | Int32 | Cellkolumnindex. |

### Returvärde

[`Comment`](../../comment/) object index.

### Exempel

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

### Se även

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Lägger till en kommentar i samlingen.

```csharp
public int Add(string cellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Cellnamn. |

### Returvärde

[`Comment`](../../comment/) object index.

### Exempel

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

### Se även

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


