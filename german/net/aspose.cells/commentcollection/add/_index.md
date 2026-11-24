---
title: "CommentCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CommentCollection-Methode. Fügt einen Kommentar zur Sammlung hinzu"
type: docs
url: /de/net/aspose.cells/commentcollection/add/
---
## Add(int, int) {#add}

Fügt der Sammlung einen Kommentar hinzu.

```csharp
public int Add(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex der Zelle. |
| column | Int32 | Spaltenindex der Zelle. |

### Rückgabewert

[`Comment`](../../comment/) object index.

### Beispiele

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

### Siehe auch

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Fügt der Sammlung einen Kommentar hinzu.

```csharp
public int Add(string cellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Zellname. |

### Rückgabewert

[`Comment`](../../comment/) object index.

### Beispiele

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

### Siehe auch

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


