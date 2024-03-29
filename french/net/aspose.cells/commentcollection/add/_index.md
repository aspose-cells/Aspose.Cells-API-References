---
title: Add
second_title: Référence de l'API Aspose.Cells pour .NET
description: Ajoute un commentaire à la collection.
type: docs
weight: 20
url: /fr/net/aspose.cells/commentcollection/add/
---
## Add(int, int) {#add}

Ajoute un commentaire à la collection.

```csharp
public int Add(int row, int column)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| row | Int32 | Index de ligne de cellule. |
| column | Int32 | Indice de colonne de cellule. |

### Return_Value

[`Comment`](../../comment) indice d'objet.

### Exemples

```csharp

[C#]
int commentIndex1 = comments.Add(0, 0);
Comment comment1 = comments[commentIndex1];
comment1.Note = "First note.";
comment1.Font.Name = "Times New Roman";
```

### Voir également

* class [CommentCollection](../../commentcollection)
* espace de noms [Aspose.Cells](../../commentcollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Ajoute un commentaire à la collection.

```csharp
public int Add(string cellName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| cellName | String | Nom de la cellule. |

### Return_Value

[`Comment`](../../comment) indice d'objet.

### Exemples

```csharp

[C#]
int commentIndex2 = comments.Add("B2");
Comment comment2 = comments[commentIndex2];
comment2.Note = "Second note.";
comment2.Font.Name = "Times New Roman";
```

### Voir également

* class [CommentCollection](../../commentcollection)
* espace de noms [Aspose.Cells](../../commentcollection)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
