---
title: "CommentCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CommentCollection-egenskapen. Hämtar Comment-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells/commentcollection/item/
---
## CommentCollection indexer (1 of 3)

Hämtar [`Comment`](../../comment/) elementet på det angivna indexet.

```csharp
public Comment this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till kommentarer till celler
            int commentIndex1 = worksheet.Comments.Add("A1");
            int commentIndex2 = worksheet.Comments.Add("B2");
            
            // Kom åt kommentarer med Item-egenskapen
            Comment comment1 = worksheet.Comments[commentIndex1];
            Comment comment2 = worksheet.Comments[commentIndex2];
            
            // Ange kommentarsanteckningar
            comment1.Note = "First comment";
            comment2.Note = "Second comment";
            
            // Ändra den första kommentaren med Item-egenskapen
            worksheet.Comments[0].Note = "Updated first comment";
            
            // Kom åt och ändra kommentar direkt från samlingen
            Comment comment3 = worksheet.Comments[1];
            comment3.Note = "Updated second comment";
            
            // Spara arbetsboken
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (2 of 3)

Hämtar [`Comment`](../../comment/) elementet på den angivna cellen.

```csharp
public Comment this[string cellName] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| cellName | Cellnamn. |

### Returvärde

Elementet på den angivna cellen.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till kommentarer i celler med cellreferenser
            int comment1Index = worksheet.Comments.Add(0, 0); // A1
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add(1, 1); // B2
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add(2, 2); // C3
            worksheet.Comments[comment3Index].Note = "Third comment";

            // Kom åt kommentarer med Item-egenskapen med cellreferenser
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments["A1"];
            Comment comment2 = comments["B2"];
            Comment comment3 = comments["C3"];

            // Ändra kommentarsanteckningar
            comment1.Note = "Updated first note";
            comment2.Note = "Updated second note";
            comment3.Note = "Updated third note";

            // Spara arbetsboken
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (3 of 3)

Hämtar [`Comment`](../../comment/) elementet på det angivna radindexet och kolumnindexet.

```csharp
public Comment this[int row, int column] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| row | Radindex. |
| column | Kolumnindex. |

### Returvärde

Elementet på den angivna cellen.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till kommentarer i celler med cellreferenser
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";

            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";

            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";

            // Kom åt kommentarer med Item-egenskapen med rad-/kolumnindex
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments[0, 0];
            comment1.Note = "Updated first comment";

            Comment comment2 = comments[1, 1];
            comment2.Note = "Updated second comment";

            // Spara arbetsboken
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


