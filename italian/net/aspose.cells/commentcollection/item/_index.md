---
title: "CommentCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CommentCollection. Ottiene l'elemento Comment all'indice specificato"
type: docs
url: /it/net/aspose.cells/commentcollection/item/
---
## CommentCollection indexer (1 of 3)

Ottiene l'elemento [`Comment`](../../comment/) all'indice specificato.

```csharp
public Comment this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi commenti alle celle
            int commentIndex1 = worksheet.Comments.Add("A1");
            int commentIndex2 = worksheet.Comments.Add("B2");
            
            // Accedi ai commenti usando la proprietà Item
            Comment comment1 = worksheet.Comments[commentIndex1];
            Comment comment2 = worksheet.Comments[commentIndex2];
            
            // Imposta le note del commento
            comment1.Note = "First comment";
            comment2.Note = "Second comment";
            
            // Modifica il primo commento usando la proprietà Item
            worksheet.Comments[0].Note = "Updated first comment";
            
            // Accedi e modifica il commento direttamente dalla collezione
            Comment comment3 = worksheet.Comments[1];
            comment3.Note = "Updated second comment";
            
            // Salva la cartella di lavoro
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (2 of 3)

Ottiene l'elemento [`Comment`](../../comment/) nella cella specificata.

```csharp
public Comment this[string cellName] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| cellName | Nome della cella. |

### Valore di ritorno

L'elemento nella cella specificata.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi commenti alle celle usando i riferimenti di cella
            int comment1Index = worksheet.Comments.Add(0, 0); // A1
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add(1, 1); // B2
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add(2, 2); // C3
            worksheet.Comments[comment3Index].Note = "Third comment";

            // Accedi ai commenti usando la proprietà Item con riferimenti di cella
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments["A1"];
            Comment comment2 = comments["B2"];
            Comment comment3 = comments["C3"];

            // Modifica le note dei commenti
            comment1.Note = "Updated first note";
            comment2.Note = "Updated second note";
            comment3.Note = "Updated third note";

            // Salva la cartella di lavoro
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (3 of 3)

Ottiene l'elemento [`Comment`](../../comment/) all'indice di riga e colonna specificati.

```csharp
public Comment this[int row, int column] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| riga | Indice della riga. |
| colonna | Indice colonna. |

### Valore di ritorno

L'elemento nella cella specificata.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi commenti alle celle usando i riferimenti di cella
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";

            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";

            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";

            // Accedi ai commenti usando la proprietà Item con indici di riga/colonna
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments[0, 0];
            comment1.Note = "Updated first comment";

            Comment comment2 = comments[1, 1];
            comment2.Note = "Updated second comment";

            // Salva la cartella di lavoro
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


