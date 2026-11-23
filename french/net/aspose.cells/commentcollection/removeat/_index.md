---
title: "CommentCollection.RemoveAt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CommentCollection. Supprime le commentaire de la cellule spécifique"
type: docs
url: /fr/net/aspose.cells/commentcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

Supprime le commentaire de la cellule spécifique.

```csharp
public void RemoveAt(string cellName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Le nom de la cellule qui contient un commentaire. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des commentaires aux cellules en utilisant les noms de cellules
            int commentIndex1 = worksheet.Comments.Add("A1");
            worksheet.Comments[commentIndex1].Note = "Comment in A1";
            
            int commentIndex2 = worksheet.Comments.Add("B2");
            worksheet.Comments[commentIndex2].Note = "Comment in B2";
            
            int commentIndex3 = worksheet.Comments.Add("C3");
            worksheet.Comments[commentIndex3].Note = "Comment in C3";
            
            // Supprimer le commentaire de la cellule B2 en utilisant RemoveAt avec un paramètre de chaîne
            worksheet.Comments.RemoveAt("B2");
            
            // Enregistrez le classeur
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, int) {#removeat_1}

Supprime le commentaire de la cellule spécifique.

```csharp
public void RemoveAt(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne. |
| column | Int32 | l'index de colonne. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodRemoveAtWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des commentaires aux cellules en utilisant les références de cellules
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";
            
            // Supprimer le commentaire à la ligne 1, colonne 1 (B2)
            worksheet.Comments.RemoveAt(1, 1);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


