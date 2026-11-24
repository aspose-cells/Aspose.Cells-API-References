---
title: "CommentCollection.RemoveAt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CommentCollection-Methode. Entfernt den Kommentar der spezifischen Zelle"
type: docs
url: /de/net/aspose.cells/commentcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

Entfernt den Kommentar der angegebenen Zelle.

```csharp
public void RemoveAt(string cellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Der Name der Zelle, die einen Kommentar enthält. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Kommentare zu Zellen mittels Zellnamen hinzu
            int commentIndex1 = worksheet.Comments.Add("A1");
            worksheet.Comments[commentIndex1].Note = "Comment in A1";
            
            int commentIndex2 = worksheet.Comments.Add("B2");
            worksheet.Comments[commentIndex2].Note = "Comment in B2";
            
            int commentIndex3 = worksheet.Comments.Add("C3");
            worksheet.Comments[commentIndex3].Note = "Comment in C3";
            
            // Entferne Kommentar bei Zelle B2 mittels RemoveAt mit String‑Parameter
            worksheet.Comments.RemoveAt("B2");
            
            // Speichere die Arbeitsmappe
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, int) {#removeat_1}

Entfernt den Kommentar der angegebenen Zelle.

```csharp
public void RemoveAt(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodRemoveAtWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Kommentare zu Zellen anhand von Zellreferenzen hinzu
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";
            
            // Entferne Kommentar bei Zeile 1, Spalte 1 (B2)
            worksheet.Comments.RemoveAt(1, 1);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


