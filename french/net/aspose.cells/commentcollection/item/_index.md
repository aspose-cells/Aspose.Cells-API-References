---
title: "CommentCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CommentCollection. Obtient l'élément Comment à l'index spécifié"
type: docs
url: /fr/net/aspose.cells/commentcollection/item/
---
## CommentCollection indexer (1 of 3)

Obtient l'élément [`Comment`](../../comment/) à l'index spécifié.

```csharp
public Comment this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des commentaires aux cellules
            int commentIndex1 = worksheet.Comments.Add("A1");
            int commentIndex2 = worksheet.Comments.Add("B2");
            
            // Accéder aux commentaires en utilisant la propriété Item
            Comment comment1 = worksheet.Comments[commentIndex1];
            Comment comment2 = worksheet.Comments[commentIndex2];
            
            // Définir les notes du commentaire
            comment1.Note = "First comment";
            comment2.Note = "Second comment";
            
            // Modifier le premier commentaire en utilisant la propriété Item
            worksheet.Comments[0].Note = "Updated first comment";
            
            // Accéder et modifier le commentaire directement depuis la collection
            Comment comment3 = worksheet.Comments[1];
            comment3.Note = "Updated second comment";
            
            // Enregistrez le classeur
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (2 of 3)

Obtient l'élément [`Comment`](../../comment/) à la cellule spécifiée.

```csharp
public Comment this[string cellName] { get; }
```

| Paramètre | Description |
| --- | --- |
| cellName | Nom de la cellule. |

### Valeur de retour

L'élément à la cellule spécifiée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des commentaires aux cellules en utilisant les références de cellules
            int comment1Index = worksheet.Comments.Add(0, 0); // A1
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add(1, 1); // B2
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add(2, 2); // C3
            worksheet.Comments[comment3Index].Note = "Third comment";

            // Accéder aux commentaires en utilisant la propriété Item avec des références de cellules
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments["A1"];
            Comment comment2 = comments["B2"];
            Comment comment3 = comments["C3"];

            // Modifier les notes de commentaire
            comment1.Note = "Updated first note";
            comment2.Note = "Updated second note";
            comment3.Note = "Updated third note";

            // Enregistrez le classeur
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (3 of 3)

Obtient l'élément [`Comment`](../../comment/) à l'index de ligne et d'index de colonne spécifiés.

```csharp
public Comment this[int row, int column] { get; }
```

| Paramètre | Description |
| --- | --- |
| ligne | Index de ligne. |
| column | Index de colonne. |

### Valeur de retour

L'élément à la cellule spécifiée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des commentaires aux cellules en utilisant les références de cellules
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";

            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";

            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";

            // Accéder aux commentaires en utilisant la propriété Item avec des indices de ligne/colonne
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments[0, 0];
            comment1.Note = "Updated first comment";

            Comment comment2 = comments[1, 1];
            comment2.Note = "Updated second comment";

            // Enregistrez le classeur
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


