---
title: "CommentCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CommentCollection-metod. Tar bort kommentaren för den specifika cellen"
type: docs
url: /sv/net/aspose.cells/commentcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

Tar bort kommentaren för den specifika cellen.

```csharp
public void RemoveAt(string cellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Namnet på cellen som innehåller en kommentar. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till kommentarer i celler med cellnamn
            int commentIndex1 = worksheet.Comments.Add("A1");
            worksheet.Comments[commentIndex1].Note = "Comment in A1";
            
            int commentIndex2 = worksheet.Comments.Add("B2");
            worksheet.Comments[commentIndex2].Note = "Comment in B2";
            
            int commentIndex3 = worksheet.Comments.Add("C3");
            worksheet.Comments[commentIndex3].Note = "Comment in C3";
            
            // Ta bort kommentar i cell B2 med RemoveAt och strängparameter
            worksheet.Comments.RemoveAt("B2");
            
            // Spara arbetsboken
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Se även

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, int) {#removeat_1}

Tar bort kommentaren för den specifika cellen.

```csharp
public void RemoveAt(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| column | Int32 | kolumnindexet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodRemoveAtWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till kommentarer i celler med cellreferenser
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";
            
            // Ta bort kommentar på rad 1, kolumn 1 (B2)
            worksheet.Comments.RemoveAt(1, 1);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


