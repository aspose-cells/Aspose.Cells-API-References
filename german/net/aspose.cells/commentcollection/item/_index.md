---
title: "CommentCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CommentCollection-Eigenschaft. Gibt das Comment-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/commentcollection/item/
---
## CommentCollection indexer (1 of 3)

Gibt das [`Comment`](../../comment/) Element am angegebenen Index zurück.

```csharp
public Comment this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kommentare zu Zellen hinzufügen
            int commentIndex1 = worksheet.Comments.Add("A1");
            int commentIndex2 = worksheet.Comments.Add("B2");
            
            // Zugriff auf Kommentare über die Item-Eigenschaft
            Comment comment1 = worksheet.Comments[commentIndex1];
            Comment comment2 = worksheet.Comments[commentIndex2];
            
            // Kommentarhinweise festlegen
            comment1.Note = "First comment";
            comment2.Note = "Second comment";
            
            // Ersten Kommentar über die Item-Eigenschaft ändern
            worksheet.Comments[0].Note = "Updated first comment";
            
            // Zugriff auf Kommentar und direkte Änderung aus der Sammlung
            Comment comment3 = worksheet.Comments[1];
            comment3.Note = "Updated second comment";
            
            // Speichere die Arbeitsmappe
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (2 of 3)

Gibt das [`Comment`](../../comment/) Element in der angegebenen Zelle zurück.

```csharp
public Comment this[string cellName] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| cellName | Zellname. |

### Rückgabewert

Das Element in der angegebenen Zelle.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Kommentare zu Zellen anhand von Zellreferenzen hinzu
            int comment1Index = worksheet.Comments.Add(0, 0); // A1
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add(1, 1); // B2
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add(2, 2); // C3
            worksheet.Comments[comment3Index].Note = "Third comment";

            // Zugriff auf Kommentare über die Item-Eigenschaft mit Zellreferenzen
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments["A1"];
            Comment comment2 = comments["B2"];
            Comment comment3 = comments["C3"];

            // Kommentarhinweise ändern
            comment1.Note = "Updated first note";
            comment2.Note = "Updated second note";
            comment3.Note = "Updated third note";

            // Speichere die Arbeitsmappe
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (3 of 3)

Gibt das [`Comment`](../../comment/) Element am angegebenen Zeilenindex und Spaltenindex zurück.

```csharp
public Comment this[int row, int column] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| row | Zeilenindex. |
| column | Spaltenindex. |

### Rückgabewert

Das Element in der angegebenen Zelle.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Kommentare zu Zellen anhand von Zellreferenzen hinzu
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";

            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";

            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";

            // Zugriff auf Kommentare über die Item-Eigenschaft mit Zeilen-/Spaltenindizes
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments[0, 0];
            comment1.Note = "Updated first comment";

            Comment comment2 = comments[1, 1];
            comment2.Note = "Updated second comment";

            // Speichere die Arbeitsmappe
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


